#!groovy

def builder = new Builder(this, '0f11d4d1-6557-423c-b5ae-693cc87f7b4b')
builder.gitClone(['https://github.com/VEuPathDB/test_service.git': env.BRANCH])
builder.buildContainers([[name: 'test_service', path: '.']])
