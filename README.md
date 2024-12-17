# devops-netology

## Файлы, проигнорированные с помощью .gitignore

1. **.gitignore** в корневом каталоге в нынешнем (пустом) виде никак не ограничивает отслежвание файлов

2. **.gitignore** в каталоге `terraform` действует внутри данного и вложенных каталогов (на корень никакого влияния не оказывает)
`**/.terraform/*` - игнорируются все файлы внутри папки .terraform вложенной непосредственно в папку terraform или глубже
`*.tfstate, *.tfstate.*` - игнорируются все файлы с "расширением" tfstate либо tfstate.\* внутри папки terraform
`crash.log, crash.*.log` - здесь все понятно понятно, данные файлы внутри папки terraform
`*.tfvars, *.tfvars.json` - любые файлы с расширениями tfvars либо tfvars.json внутри папки terraform
`override.tf, override.tf.json, *_override.tf, *_override.tf.json` - файлы override.tf, override.tf.json и любые файлы с постфиксами  \_override.rf или \_override.tf.json внутри папки terraform
`.terraform.tfstate.lock.info` - данный файл внутри папки terraform
`.terraformrc, terraform.rc` - данные фалы внутри папки terraform
