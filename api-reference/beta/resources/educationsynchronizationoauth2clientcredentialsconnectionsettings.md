---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 当 OAuth2 客户端凭据授予以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 8cf7ee292b819a05a735ce6bed2a2c4fc4275907
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425454"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="85539-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="85539-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

> <span data-ttu-id="85539-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85539-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85539-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85539-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="85539-106">当[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="85539-106">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="85539-107">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="85539-107">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="85539-108">属性</span><span class="sxs-lookup"><span data-stu-id="85539-108">Properties</span></span>

| <span data-ttu-id="85539-109">属性</span><span class="sxs-lookup"><span data-stu-id="85539-109">Property</span></span> | <span data-ttu-id="85539-110">类型</span><span class="sxs-lookup"><span data-stu-id="85539-110">Type</span></span> | <span data-ttu-id="85539-111">说明</span><span class="sxs-lookup"><span data-stu-id="85539-111">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="85539-112">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="85539-112">**tokenUrl**</span></span> | <span data-ttu-id="85539-113">String</span><span class="sxs-lookup"><span data-stu-id="85539-113">String</span></span> | <span data-ttu-id="85539-114">要获取访问令牌的数据提供程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="85539-114">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="85539-115">**scope**</span><span class="sxs-lookup"><span data-stu-id="85539-115">**scope**</span></span> | <span data-ttu-id="85539-116">String</span><span class="sxs-lookup"><span data-stu-id="85539-116">String</span></span> | <span data-ttu-id="85539-117">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="85539-117">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="85539-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85539-118">JSON representation</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "#microsoft.graph.educationSynchronizationOAuth2ClientCredentialsConnectionSettings"
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
