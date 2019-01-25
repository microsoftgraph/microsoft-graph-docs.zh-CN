---
title: educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源
description: 当 OAuth2 客户端凭据授予以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 37121868793dd76aec2c3b48182e114348d21014
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523552"
---
# <a name="educationsynchronizationoauth2clientcredentialsconnectionsettings-resource"></a><span data-ttu-id="f2f38-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings 资源</span><span class="sxs-lookup"><span data-stu-id="f2f38-103">educationSynchronizationOAuth2ClientCredentialsConnectionSettings resource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2f38-104">当[OAuth2 客户端凭据授予](https://tools.ietf.org/html/rfc6749#section-4.4)以用于连接到的数据提供程序时，应使用此连接设置类型设置配置文件。</span><span class="sxs-lookup"><span data-stu-id="f2f38-104">When [OAuth2 Client Credentials Grant](https://tools.ietf.org/html/rfc6749#section-4.4) is to be used to connect to the data provider, this connection settings type should be used to set up the profile.</span></span>

<span data-ttu-id="f2f38-105">派生自[educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="f2f38-105">Derived from [educationSynchronizationConnectionSettings](educationsynchronizationconnectionsettings.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f2f38-106">属性</span><span class="sxs-lookup"><span data-stu-id="f2f38-106">Properties</span></span>

| <span data-ttu-id="f2f38-107">属性</span><span class="sxs-lookup"><span data-stu-id="f2f38-107">Property</span></span> | <span data-ttu-id="f2f38-108">类型</span><span class="sxs-lookup"><span data-stu-id="f2f38-108">Type</span></span> | <span data-ttu-id="f2f38-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2f38-109">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="f2f38-110">**tokenUrl**</span><span class="sxs-lookup"><span data-stu-id="f2f38-110">**tokenUrl**</span></span> | <span data-ttu-id="f2f38-111">String</span><span class="sxs-lookup"><span data-stu-id="f2f38-111">String</span></span> | <span data-ttu-id="f2f38-112">要获取访问令牌的数据提供程序的 URL。</span><span class="sxs-lookup"><span data-stu-id="f2f38-112">The URL to get access tokens for the data provider.</span></span> |
| <span data-ttu-id="f2f38-113">**scope**</span><span class="sxs-lookup"><span data-stu-id="f2f38-113">**scope**</span></span> | <span data-ttu-id="f2f38-114">String</span><span class="sxs-lookup"><span data-stu-id="f2f38-114">String</span></span> | <span data-ttu-id="f2f38-115">[访问请求的范围](https://tools.ietf.org/html/rfc6749#section-3.3)。</span><span class="sxs-lookup"><span data-stu-id="f2f38-115">[The scope of the access request](https://tools.ietf.org/html/rfc6749#section-3.3).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f2f38-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2f38-116">JSON representation</span></span>
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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationoauth2clientcredentialsconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
