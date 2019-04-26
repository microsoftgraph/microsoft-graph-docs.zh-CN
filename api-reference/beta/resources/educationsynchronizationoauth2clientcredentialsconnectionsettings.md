---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序, 则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 5b0229ae431c02f85d393ff80b0bba32e32683c9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334027"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="2d333-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="2d333-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2d333-104">如果要使用[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)连接到数据提供程序, 则此连接设置类型应用于设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="2d333-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="2d333-105">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="2d333-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="2d333-106">属性</span><span class="sxs-lookup"><span data-stu-id="2d333-106">Properties</span></span>

| <span data-ttu-id="2d333-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d333-107">Property</span></span> | <span data-ttu-id="2d333-108">类型</span><span class="sxs-lookup"><span data-stu-id="2d333-108">Type</span></span> | <span data-ttu-id="2d333-109">说明</span><span class="sxs-lookup"><span data-stu-id="2d333-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="2d333-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="2d333-110">**tokenUrl**</span></span> | <span data-ttu-id="2d333-111">String</span><span class="sxs-lookup"><span data-stu-id="2d333-111">String</span></span> | <span data-ttu-id="2d333-112">用于获取数据提供程序的访问令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="2d333-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="2d333-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="2d333-113">**scope**</span></span> | <span data-ttu-id="2d333-114">String</span><span class="sxs-lookup"><span data-stu-id="2d333-114">String</span></span> | <span data-ttu-id="2d333-115">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="2d333-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2d333-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d333-116">JSON representation</span></span>
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
