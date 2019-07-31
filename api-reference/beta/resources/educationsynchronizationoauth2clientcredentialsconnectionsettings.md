---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序, 则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ffc3af93a90ba0d6991007a64d24b9fb776e8bc8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972367"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="ea098-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="ea098-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea098-104">如果要使用[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)连接到数据提供程序, 则此连接设置类型应用于设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="ea098-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="ea098-105">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="ea098-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ea098-106">属性</span><span class="sxs-lookup"><span data-stu-id="ea098-106">Properties</span></span>

| <span data-ttu-id="ea098-107">属性</span><span class="sxs-lookup"><span data-stu-id="ea098-107">Property</span></span> | <span data-ttu-id="ea098-108">类型</span><span class="sxs-lookup"><span data-stu-id="ea098-108">Type</span></span> | <span data-ttu-id="ea098-109">说明</span><span class="sxs-lookup"><span data-stu-id="ea098-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ea098-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="ea098-110">**tokenUrl**</span></span> | <span data-ttu-id="ea098-111">String</span><span class="sxs-lookup"><span data-stu-id="ea098-111">String</span></span> | <span data-ttu-id="ea098-112">用于获取数据提供程序的访问令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="ea098-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="ea098-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="ea098-113">**scope**</span></span> | <span data-ttu-id="ea098-114">String</span><span class="sxs-lookup"><span data-stu-id="ea098-114">String</span></span> | <span data-ttu-id="ea098-115">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="ea098-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ea098-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea098-116">JSON representation</span></span>
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
