---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 如果要使用 OAuth2 客户端凭据授予连接到数据提供程序，则此连接设置类型应用于设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: dfe0a2fda8d49bd003a6ea2c23eb6a31ce619234
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289437"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="ecd81-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="ecd81-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

<span data-ttu-id="ecd81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecd81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecd81-105">如果要使用[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)连接到数据提供程序，则此连接设置类型应用于设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="ecd81-105">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="ecd81-106">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="ecd81-106">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ecd81-107">属性</span><span class="sxs-lookup"><span data-stu-id="ecd81-107">Properties</span></span>

| <span data-ttu-id="ecd81-108">属性</span><span class="sxs-lookup"><span data-stu-id="ecd81-108">Property</span></span> | <span data-ttu-id="ecd81-109">类型</span><span class="sxs-lookup"><span data-stu-id="ecd81-109">Type</span></span> | <span data-ttu-id="ecd81-110">说明</span><span class="sxs-lookup"><span data-stu-id="ecd81-110">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ecd81-111">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="ecd81-111">**tokenUrl**</span></span> | <span data-ttu-id="ecd81-112">String</span><span class="sxs-lookup"><span data-stu-id="ecd81-112">String</span></span> | <span data-ttu-id="ecd81-113">用于获取数据提供程序的访问令牌的 URL。</span><span class="sxs-lookup"><span data-stu-id="ecd81-113">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="ecd81-114">**scope**</span><span class="sxs-lookup"><span data-stu-id="ecd81-114">**scope**</span></span> | <span data-ttu-id="ecd81-115">String</span><span class="sxs-lookup"><span data-stu-id="ecd81-115">String</span></span> | <span data-ttu-id="ecd81-116">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="ecd81-116">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecd81-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecd81-117">JSON representation</span></span>
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
