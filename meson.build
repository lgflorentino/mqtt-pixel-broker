project('mqtt-pixel-broker', 'cpp', default_options : ['cpp_std=c++14'])
# boost_deps = dependency('boost', modules : ['lexical_cast', 'multi_index_container', 'multi_index'])
boost_deps = dependency('boost')
thread_dep = dependency('threads')

cmake = import('cmake')
mqtt_cpp_cmake = cmake.subproject('mqtt_cpp') 
mqtt_cpp_iface_dep = mqtt_cpp_cmake.dependency('mqtt_cpp_iface')


executable('mqtt-pixel-broker', 'source/tls_ws_server.cpp', dependencies: [boost_deps, thread_dep, mqtt_cpp_iface_dep])

