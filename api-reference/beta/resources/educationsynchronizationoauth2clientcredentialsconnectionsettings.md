---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序，则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: a6a25f63c5daef72c436fe0a9a21f4d795667602
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47989625"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="73064-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="73064-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="73064-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73064-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73064-105">如果要使用 [OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4) 连接到数据提供程序，则此连接设置类型应用于设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="73064-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="73064-106">派生自 [educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="73064-106">Derived from [educationSynchronizationConnectionSettings].</span></span>

## <a name="properties"></a><span data-ttu-id="73064-107">属性</span><span class="sxs-lookup"><span data-stu-id="73064-107">Properties</span></span>

| <span data-ttu-id="73064-108">属性</span><span class="sxs-lookup"><span data-stu-id="73064-108">Property</span></span>     | <span data-ttu-id="73064-109">类型</span><span class="sxs-lookup"><span data-stu-id="73064-109">Type</span></span>   | <span data-ttu-id="73064-110">说明</span><span class="sxs-lookup"><span data-stu-id="73064-110">Description</span></span>                                                                                                                |
| :----------- | :----- | :------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="73064-111">clientId</span><span class="sxs-lookup"><span data-stu-id="73064-111">clientId</span></span>     | <span data-ttu-id="73064-112">字符串</span><span class="sxs-lookup"><span data-stu-id="73064-112">String</span></span> | <span data-ttu-id="73064-113">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="73064-113">Client ID used to connect to the provider.</span></span> <span data-ttu-id="73064-114">继承自 [educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="73064-114">Inherited from [educationSynchronizationConnectionSettings].</span></span>                    |
| <span data-ttu-id="73064-115">clientSecret</span><span class="sxs-lookup"><span data-stu-id="73064-115">clientSecret</span></span> | <span data-ttu-id="73064-116">字符串</span><span class="sxs-lookup"><span data-stu-id="73064-116">String</span></span> | <span data-ttu-id="73064-117">用于对与提供程序的连接进行身份验证的客户端密码。</span><span class="sxs-lookup"><span data-stu-id="73064-117">Client secret to authenticate the connection to the provider.</span></span> <span data-ttu-id="73064-118">继承自 [educationSynchronizationConnectionSettings]。</span><span class="sxs-lookup"><span data-stu-id="73064-118">Inherited from [educationSynchronizationConnectionSettings].</span></span> |
| <span data-ttu-id="73064-119">tokenUrl</span><span class="sxs-lookup"><span data-stu-id="73064-119">tokenUrl</span></span>     | <span data-ttu-id="73064-120">String</span><span class="sxs-lookup"><span data-stu-id="73064-120">String</span></span> | <span data-ttu-id="73064-121">用于获取数据提供程序的访问令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="73064-121">The URL to get access tokens for the data provider.</span></span>                                                                        |
| <span data-ttu-id="73064-122">scope</span><span class="sxs-lookup"><span data-stu-id="73064-122">scope</span></span>        | <span data-ttu-id="73064-123">String</span><span class="sxs-lookup"><span data-stu-id="73064-123">String</span></span> | <span data-ttu-id="73064-124">访问请求的作用域 (请参阅 [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)) 。</span><span class="sxs-lookup"><span data-stu-id="73064-124">The scope of the access request (see [RFC6749](https://tools.ietf.org/html/rfc6749#section-3.3)).</span></span>                          |

[educationsynchronizationconnectionsettings]: educationsynchronizationconnectionsettings.md

## <a name="json-representation"></a><span data-ttu-id="73064-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73064-126">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
{
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
  "clientId": "String",
  "clientSecret": "String",
  "tokenUrl": "String",
  "scope": "String"
}
```


