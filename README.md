[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"
![valid XHTML][checkmark]

# Mozg\CheckoutFilters

--

Filtros

--

Filtre seus métodos de pagamento e envio.

Pagamento
-------

- Filtrar por grupo de clientes
- Filtrar por idade do cliente
- Ocultar outros métodos de pagamento se o total geral for zero

Envio
-------

- Filtrar por grupo de clientes

--

Restrições

--

Restrinja salvar o endereço de faturamento caso a data de nascimento fornecida seja inferior a 18 anos.

--

Restrinja a exibição do método de entrega caso o serviço do Correios esteja on-line

--

## Instalação - Atualização - Desinstalação - Desativação

Este módulo destina-se a ser instalado usando o [Composer][getcomposer]

Antes de executar os processos, [clique aqui][requerimentos] e leia os pré-requisitos e sugestões

--

Certique se da existencia do arquivo composer.json na raiz do projeto Magento e que o mesmo tenha os trechos "minimum-stability", "prefer-stable", "repositories" e '"magento-root-dir":"./"', conforme https://gist.github.com/mozgbrasil/0c9bb8792ea6273ea24aed30b0fbcfba

Caso não exista o arquivo composer.json na raiz do projeto Magento, efetue o download

	wget https://gist.githubusercontent.com/mozgbrasil/0c9bb8792ea6273ea24aed30b0fbcfba/raw/9b514bc896171b6d75833b6f165065356f62ca59/composer.json

--

Para qualquer atualização no Magento sempre mantenha o Compiler e o Cache desativado

--

### Para instalar o módulo execute o comando a seguir no terminal do seu servidor no diretório do seu projeto

	composer require mozgbrasil/magento-checkout-filters-php56:dev-master

Você pode verificar se o módulo está instalado, indo ao backend em:

	STORES -> Configuration -> ADVANCED/Advanced -> Disable Modules Output

--

### Para atualizar o módulo execute o comando a seguir no terminal do seu servidor no diretório do seu projeto

Antes de efetuar qualquer processo que envolva atualização no Magento é recomendado manter o Compiler e Cache desativado

	composer clear-cache && composer update

Na ocorrência de erro, renomeie a pasta /vendor/mozgbrasil e execute novamente

Para checar a data do módulo execute o seguinte comando

	grep -ri --include=*.json 'time": "' ./vendor/mozgbrasil

--

### Para [desinstalar][uninstall-mods] o módulo execute o comando a seguir no terminal do seu servidor no diretório do seu projeto

	composer remove mozgbrasil/magento-checkout-filters-php56 && composer clear-cache && composer update

--

### Para desativar o módulo

Renomeie a pasta do módulo

Cada módulo tem a sua pasta no diretório /vendor/mozgbrasil/

## Como configurar o método

Antes de configurar o módulo você deve cadastrar o CEP de origem, indo ao backend em:

	STORES -> Configuration -> Sales/Shipping Settings -> Origin

Para configurar o método de entrega, acesse no backend em:

	STORES -> Configuration -> Mozg -> Checkout Filters

Você terá os campos a seguir

### • **Ocultar método de pagamento para total zero**

Para "ativar" ou "desativar" o uso do método

### • **Ativar**

Para "ativar" ou "desativar" o uso do método


## Perguntas mais frequentes "FAQ"

### Sobre a restrição de exibição do método

Para o método "mozg_correios" é feito requisição onde caso o serviço esteja offline o método não deve ser exibido

É possivel definir para os metodos serem exibido somente caso o Correios esteja offline

## Contribuintes

Equipe Mozg

## License

[Comercial License](LICENSE.txt)

## Badges

[![Join the chat at https://gitter.im/mozgbrasil](https://badges.gitter.im/Join%20Chat.svg)](https://gitter.im/mozgbrasil/)
[![Latest Stable Version](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/v/stable)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![Total Downloads](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/downloads)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![Latest Unstable Version](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/v/unstable)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![License](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/license)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![Monthly Downloads](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/d/monthly)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![Daily Downloads](https://poser.pugx.org/mozgbrasil/mozgbrasil/magento-checkout-filters-php56/d/daily)](https://packagist.org/packages/mozgbrasil/mozgbrasil/magento-checkout-filters-php56)
[![Reference Status](https://www.versioneye.com/php/mozgbrasil:mozgbrasil/magento-checkout-filters-php56/reference_badge.svg?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:mozgbrasil/magento-checkout-filters-php56/references)
[![Dependency Status](https://www.versioneye.com/php/mozgbrasil:mozgbrasil/magento-checkout-filters-php56/1.0.0/badge?style=flat-square)](https://www.versioneye.com/php/mozgbrasil:mozgbrasil/magento-checkout-filters-php56/1.0.0)

:cat2:
