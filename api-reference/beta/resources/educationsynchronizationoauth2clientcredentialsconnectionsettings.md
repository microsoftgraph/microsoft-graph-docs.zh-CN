---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 当 OAuth2 客户端凭据授予以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8976c3a3a6088abd88cf70182040d4b3a6cc3f7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912888"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="361ec-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="361ec-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="361ec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="361ec-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="361ec-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="361ec-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="361ec-106">当[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="361ec-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="361ec-107">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="361ec-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="361ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="361ec-108">Properties</span></span>

| <span data-ttu-id="361ec-109">属性</span><span class="sxs-lookup"><span data-stu-id="361ec-109">Property</span></span> | <span data-ttu-id="361ec-110">类型</span><span class="sxs-lookup"><span data-stu-id="361ec-110">Type</span></span> | <span data-ttu-id="361ec-111">Description</span><span class="sxs-lookup"><span data-stu-id="361ec-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="361ec-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="361ec-112">**tokenUrl**</span></span> | <span data-ttu-id="361ec-113">字符串</span><span class="sxs-lookup"><span data-stu-id="361ec-113">String</span></span> | <span data-ttu-id="361ec-114">要获取访问令牌的数据提供程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="361ec-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="361ec-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="361ec-115">**scope**</span></span> | <span data-ttu-id="361ec-116">字符串</span><span class="sxs-lookup"><span data-stu-id="361ec-116">String</span></span> | <span data-ttu-id="361ec-117">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="361ec-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="361ec-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="361ec-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
}-->

```json
"connectionSettings": {
    "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings",
    "clientId": "String",
    "clientSecret": "String",
    "tokenUrl": "String",
    "scope": "String"
}
```
