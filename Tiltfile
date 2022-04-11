#allow_k8s_contexts(os.getenv("CURRENT_CONTEXT", default='kind-kind'))
default_registry(os.getenv("DEFAULT_REGISTRY", default='dev.local'))

#custom_build('python-accelerator:latest', '.')

load('ext://pack', 'pack')
pack('python-accelerator', path=".", builder="heroku/buildpacks:20")

k8s_yaml(['kubernetes/k8s/deployment.yaml', 'kubernetes/k8s/service.yaml'])
k8s_resource('python-accelerator', port_forwards=8080)