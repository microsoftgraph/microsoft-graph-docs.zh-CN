---
title: educationSynchronizationConnectionSettings 资源类型
description: '代表提供商连接设置。 这样，系统知道如何连接到提供程序的 Api。 '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: f6af6851e1e9d327b05c9ca1c7ed5929335a6e17
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526863"
---
# <a name="educationsynchronizationconnectionsettings-resource-type"></a><span data-ttu-id="ce9e8-104">educationSynchronizationConnectionSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce9e8-104">educationSynchronizationConnectionSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce9e8-105">代表提供商连接设置。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-105">Represents the provider connection settings.</span></span> <span data-ttu-id="ce9e8-106">这样，系统知道如何连接到提供程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-106">This allows the system to know how to connect to the provider APIs.</span></span> 

> <span data-ttu-id="ce9e8-107">**注意：** 此复杂类型是抽象类。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-107">**Note:** This complex type is abstract.</span></span> <span data-ttu-id="ce9e8-108">引用的特定类型的列出的连接设置。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-108">Refer to the specific types of connection settings listed.</span></span>

## <a name="derived-types"></a><span data-ttu-id="ce9e8-109">派生的类型</span><span class="sxs-lookup"><span data-stu-id="ce9e8-109">Derived types</span></span>
| <span data-ttu-id="ce9e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce9e8-110">Type</span></span> | <span data-ttu-id="ce9e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce9e8-111">Description</span></span> | 
|:-|:-|
| [<span data-ttu-id="ce9e8-112">**educationSynchronizationOAuth1ConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="ce9e8-112">**educationSynchronizationOAuth1ConnectionSettings**</span></span>](educationsynchronizationoauth1connectionsettings.md) | <span data-ttu-id="ce9e8-113">使用此类型提供 OAuth1 连接设置。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-113">Use this type to provide OAuth1 connection settings.</span></span> |
| [<span data-ttu-id="ce9e8-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span><span class="sxs-lookup"><span data-stu-id="ce9e8-114">**educationSynchronizationOAuth2ClientCredentialsConnectionSettings**</span></span>](educationsynchronizationoauth2clientcredentialsconnectionsettings.md) | <span data-ttu-id="ce9e8-115">使用此类型提供 OAuth2 客户端凭据授予连接设置。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-115">Use this type to provide OAuth2 Client Credentials Grant connection settings.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce9e8-116">属性</span><span class="sxs-lookup"><span data-stu-id="ce9e8-116">Properties</span></span>

| <span data-ttu-id="ce9e8-117">属性</span><span class="sxs-lookup"><span data-stu-id="ce9e8-117">Property</span></span> | <span data-ttu-id="ce9e8-118">类型</span><span class="sxs-lookup"><span data-stu-id="ce9e8-118">Type</span></span> | <span data-ttu-id="ce9e8-119">说明</span><span class="sxs-lookup"><span data-stu-id="ce9e8-119">Description</span></span> |
|:-|:-|:-|
| <span data-ttu-id="ce9e8-120">**clientId**</span><span class="sxs-lookup"><span data-stu-id="ce9e8-120">**clientId**</span></span> | <span data-ttu-id="ce9e8-121">String</span><span class="sxs-lookup"><span data-stu-id="ce9e8-121">String</span></span> |  <span data-ttu-id="ce9e8-122">用于连接到提供程序的客户端 ID。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-122">Client ID used to connect to the provider.</span></span> |
| <span data-ttu-id="ce9e8-123">client_secret</span><span class="sxs-lookup"><span data-stu-id="ce9e8-123">**clientSecret**</span></span> | <span data-ttu-id="ce9e8-124">String</span><span class="sxs-lookup"><span data-stu-id="ce9e8-124">String</span></span> |  <span data-ttu-id="ce9e8-125">验证连接到提供程序的客户端机密。</span><span class="sxs-lookup"><span data-stu-id="ce9e8-125">Client secret to authenticate the connection to the provider.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsynchronizationconnectionsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
