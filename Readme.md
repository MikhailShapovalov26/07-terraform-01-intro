# 7.1. Инфраструктура как код
## 1.
1) Так как нет чёткого ТЗ, и то будет такой ответ. Будем использовать изменяемый, так как мы не знаем что и как должно работать, так же возвожмо увелечение внешних клиентов. Из-за этого нужно чтоб наш сервис был в будущем возможно маштабировать.
2) Будет центральный сервер в проекте.
3) Если будем использовать Ansible, то агенты нам не нужны. 
4) В связи с тем, что у нас знают Anaible, то будем использовать только его..
</br>
Из списка, которым мы обладаем, я бы предложил использовать Terraform, Docker и Ansible на начальных этапах. Так как мы пока не понимаем, что будет за проект, кто наш главный клиент на первых этапах. Эти инструменты достаточно гибкие. По отдельности. Так жек мы можем готовить Kubernetes для дальнгейшего развертывания. 
В дальнейшем можно было бы использовать Chef.
Вопрос достаточно много. Будет это облако или физический сервер. Кто его будет обслуживать. Кол-во запросов, нагрузка. нужна ли БД нам. Будет ли шардирование на БД. Кол0во серверов, Сервер с хранением данных пользователей. 
# 2.

    terraform -v        
    Terraform v1.1.9
    on linux_amd64

    Your version of Terraform is out of date! The latest version
    is 1.2.3. You can update by downloading from https://www.terraform.io/downloads.html
# 3.

       ./terraform -v
        Terraform v1.0.3
        on linux_amd64

        Your version of Terraform is out of date! The latest version
        is 1.2.3. You can update by downloading from https://www.terraform.io/downloads.html
        terraform -v
        Terraform v1.1.9
        on linux_amd64

        Your version of Terraform is out of date! The latest version
        is 1.2.3. You can update by downloading from https://www.terraform.io/downloads.html

