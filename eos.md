---
layout: ecosystem
title: EOS DeFi ecosystem
metadescription: List of the best EOS Defi Products. DeFi is the movement that leverages decentralized networks to transform old financial products into trustless and transparent protocols that run without intermediaries.
permalink: eos
h1title: EOS DeFi ecosystem
pagetitle: EOS DeFi ecosystem - List of the best EOS Defi Projects
featured-image: /images/og-eos.png

---

{% assign counter = 0 %}
{% assign counter_eth = 0 %}
{% assign counter_btc = 0 %}
{% assign counter_eos = 0 %}
{% assign counter_tron = 0 %}
{% assign counter_stellar = 0 %}

{% for assets-managament-tools in site.assets-managament-tools  %}
{% if assets-managament-tools.ecosystem contains 'ethereum' %}  {% assign counter_eth = counter_eth | plus: 1 %}
 {% endif %}
{% if assets-managament-tools.ecosystem contains 'bitcoin' %} {% endif %}
{% if assets-managament-tools.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}

{% assign counter = counter | plus: 1 %}


{% endfor %}


{% for derivatives in site.derivatives %}
{% if derivatives.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if derivatives.ecosystem contains 'bitcoin' %} {% endif %}
{% if derivatives.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for exchanges in site.exchanges %}
{% if exchanges.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if exchanges.ecosystem contains 'bitcoin' %} {% endif %}
{% if exchanges.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if exchanges.ecosystem contains 'tron' %} {% endif %}
{% if exchanges.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for infrastructure in site.infrastructure %}
{% if infrastructure.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if infrastructure.ecosystem contains 'bitcoin' %} {% endif %}
{% if infrastructure.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if infrastructure.ecosystem contains 'tron' %} {% endif %}
{% if infrastructure.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for insurance in site.insurance %}
{% if insurance.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if insurance.ecosystem contains 'bitcoin' %} {% endif %}
{% if insurance.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if insurance.ecosystem contains 'tron' %} {% endif %}
{% if insurance.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for assets-tokenization in site.assets-tokenization %}
{% if assets-tokenization.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if assets-tokenization.ecosystem contains 'bitcoin' %} {% endif %}
{% if assets-tokenization.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if assets-tokenization.ecosystem contains 'tron' %} {% endif %}
{% if assets-tokenization.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for kyc_identity in site.kyc_identity %}
{% if kyc_identity.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if kyc_identity.ecosystem contains 'bitcoin' %} {% endif %}
{% if kyc_identity.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if kyc_identity.ecosystem contains 'tron' %} {% endif %}
{% if kyc_identity.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}



{% for lending in site.lending %}
{% if lending.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if lending.ecosystem contains 'bitcoin' %} {% endif %}
{% if lending.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for marketplaces in site.marketplaces %}
{% if marketplaces.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if marketplaces.ecosystem contains 'bitcoin' %} {% endif %}
{% if marketplaces.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if marketplaces.ecosystem contains 'tron' %} {% endif %}
{% if marketplaces.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for prediction_markets in site.prediction_markets %}
{% if prediction_markets.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if prediction_markets.ecosystem contains 'bitcoin' %} {% endif %}
{% if prediction_markets.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if prediction_markets.ecosystem contains 'tron' %} {% endif %}
{% if prediction_markets.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for stablecoins in site.stablecoins %}
{% if stablecoins.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if stablecoins.ecosystem contains 'bitcoin' %} {% endif %}
{% if stablecoins.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}
{% if stablecoins.ecosystem contains 'tron' %} {% endif %}
{% if stablecoins.ecosystem contains 'stellar' %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}


{% for analytics in site.analytics %}
{% if analytics.ecosystem contains 'ethereum' %} {% assign counter_eth = counter_eth | plus: 1 %} {% endif %}
{% if analytics.ecosystem contains 'bitcoin' %} {% endif %}
{% if analytics.ecosystem contains 'eos' %} {% assign counter_eos = counter_eos | plus: 1 %} {% endif %}

{% assign counter = counter | plus: 1 %}

{% endfor %}

DeFi is the movement that leverages decentralized networks to transform old financial products into trustless and transparent protocols that run without intermediaries. We have {{ counter }} DeFi projects listed and {{ counter_eos }} of them built on EOS.


# Assets Management Tools

{% for assets-managament-tools in site.assets-managament-tools  %}
{% if assets-managament-tools.ecosystem contains 'eos' %}
### <a href="{{ assets-managament-tools.product-url }}?ref=defiprime.com">{{ assets-managament-tools.product-title }}</a>{% if assets-managament-tools.ecosystem contains 'ethereum' %} ![](images/ether.png "Built on Ethereum or related to Ethereum ecosystem"){% endif %} {% if assets-managament-tools.ecosystem contains 'bitcoin' %} ![](/images/btc.png "Using Bitcoin ecosystem"){% endif %} {% if assets-managament-tools.ecosystem contains 'eos' %} ![](/images/eos.png "Built on EOS or related to EOS ecosystem"){% endif %} {% if  assets-managament-tools.platform contains 'ios' %}    <i class="fab fa-app-store-ios" title="Mobile wallet for iOS"></i> {% endif %}  {% if  assets-managament-tools.platform contains 'android' %}    <i class="fab fa-android" title="Mobile wallet for Android"></i> {% endif %} {% if  assets-managament-tools.platform contains 'web' %}    <i class="fab fa-chrome" title="Browser based wallet"></i> {% endif %} {% if  assets-managament-tools.platform contains 'win' %}    <i class="fab fa-windows" title="Desktop wallet for windows"></i> {% endif %} {% if  assets-managament-tools.platform contains 'mac' %}    <i class="fab fa-apple" title="Desktop wallet for osx"></i> {% endif %}


{{ assets-managament-tools.product-description }}
{% endif %}
{% endfor %}

# Decentralized exchanges on EOS

{% for exchanges in site.exchanges %}
{% if exchanges.ecosystem contains 'eos' %}
### <a href="{{ exchanges.product-url }}?ref=defiprime.com">{{ exchanges.product-title }}</a>{% if exchanges.ecosystem contains 'ethereum' %} ![](images/ether.png "Built on Ethereum or related to Ethereum ecosystem"){% endif %} {% if exchanges.ecosystem contains 'bitcoin' %} ![](/images/btc.png "Using Bitcoin ecosystem"){% endif %} {% if exchanges.ecosystem contains 'eos' %} ![](/images/eos.png "Built on EOS or related to EOS ecosystem"){% endif %}{% if exchanges.ecosystem contains 'tron' %} ![](/images/tron.png "Built on Tron or related to Tron ecosystem"){% endif %}{% if exchanges.ecosystem contains 'stellar' %} ![](/images/stellar.png "Built on Stellar or related to Stellar ecosystem"){% endif %}{% if exchanges.type == 'non-custodial' %}<i class="fas fa-user-lock" title="Non-custodial"></i>{% endif %}


{{ exchanges.product-description }}
{% endif %}
{% endfor %}


# DeFi Infrastructure

{% for infrastructure in site.infrastructure %}
{% if infrastructure.ecosystem contains 'eos' %}
### <a href="{{ infrastructure.product-url }}?ref=defiprime.com">{{ infrastructure.product-title }}</a>{% if infrastructure.ecosystem contains 'ethereum' %} ![](images/ether.png "Built on Ethereum or related to Ethereum ecosystem"){% endif %} {% if infrastructure.ecosystem contains 'bitcoin' %} ![](/images/btc.png "Using Bitcoin ecosystem"){% endif %} {% if infrastructure.ecosystem contains 'eos' %} ![](/images/eos.png "Built on EOS or related to EOS ecosystem"){% endif %}{% if infrastructure.ecosystem contains 'tron' %} ![](/images/tron.png "Built on Tron or related to Tron ecosystem"){% endif %}{% if infrastructure.ecosystem contains 'stellar' %} ![](/images/stellar.png "Built on Stellar or related to Stellar ecosystem"){% endif %}


{{ infrastructure.product-description }}
{% endif %}
{% endfor %}


# Decentralized Lending on EOS

{% for lending in site.lending %}
{% if lending.ecosystem contains 'eos' %}
### <a href="{{ lending.product-url }}?ref=defiprime.com">{{ lending.product-title }}</a>{% if lending.ecosystem contains 'ethereum' %} ![](images/ether.png "Built on Ethereum or related to Ethereum ecosystem") {% endif %} {% if lending.ecosystem contains 'bitcoin' %} ![](/images/btc.png "Using Bitcoin ecosystem"){% endif %} {% if lending.ecosystem contains 'eos' %} ![](/images/eos.png "Built on EOS or related to EOS ecosystem"){% endif %}{% if lending.type == 'non-custodial' %}<i class="fas fa-user-lock" title="Non-custodial"></i>{% endif %} {% if lending.type contains 'cefi' %}<i class="fas fa-bullseye" title="CeFi product. CeFi products are custodial, use centralized price feeds, initiate margin calls centrally, centrally determine interest rates, and centrally provide liquidity for their margin calls."></i>{% endif %}


{{ lending.product-description }}
{% endif %}
{% endfor %}

# Stablecoins

{% for stablecoins in site.stablecoins %}
{% if stablecoins.ecosystem contains 'eos' %}
### <a href="{{ stablecoins.product-url }}?ref=defiprime.com">{{ stablecoins.product-title }}</a>{% if stablecoins.ecosystem contains 'ethereum' %} ![](images/ether.png "Built on Ethereum or related to Ethereum ecosystem"){% endif %} {% if stablecoins.ecosystem contains 'bitcoin' %} ![](/images/btc.png "Using Bitcoin ecosystem"){% endif %} {% if stablecoins.ecosystem contains 'eos' %} ![](/images/eos.png "Built on EOS or related to EOS ecosystem"){% endif %}{% if stablecoins.ecosystem contains 'tron' %} ![](/images/tron.png "Built on Tron or related to Tron ecosystem"){% endif %}{% if stablecoins.ecosystem contains 'stellar' %} ![](/images/stellar.png "Built on Stellar or related to Stellar ecosystem"){% endif %}


{{ stablecoins.product-description }}
{% endif %}
{% endfor %}
