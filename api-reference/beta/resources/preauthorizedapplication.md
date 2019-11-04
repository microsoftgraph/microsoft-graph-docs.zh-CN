---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: c741c303ee9ffaf18db5fc01181702f963e39ccc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939780"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="aacee-103">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="aacee-103">preAuthorizedApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aacee-104">列出使用指定权限预授权的客户端应用程序，以访问此应用程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="aacee-104">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="aacee-105">用户无需同意任何预先授权的应用程序（针对指定的权限）。</span><span class="sxs-lookup"><span data-stu-id="aacee-105">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="aacee-106">但是，preAuthorizedApplications 中未列出的任何其他权限（例如，通过增量许可请求）将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="aacee-106">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="aacee-107">属性</span><span class="sxs-lookup"><span data-stu-id="aacee-107">Properties</span></span>

| <span data-ttu-id="aacee-108">属性</span><span class="sxs-lookup"><span data-stu-id="aacee-108">Property</span></span> | <span data-ttu-id="aacee-109">类型</span><span class="sxs-lookup"><span data-stu-id="aacee-109">Type</span></span> | <span data-ttu-id="aacee-110">描述</span><span class="sxs-lookup"><span data-stu-id="aacee-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="aacee-111">appId</span><span class="sxs-lookup"><span data-stu-id="aacee-111">appId</span></span>|<span data-ttu-id="aacee-112">String</span><span class="sxs-lookup"><span data-stu-id="aacee-112">String</span></span>| <span data-ttu-id="aacee-113">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aacee-113">The unique identifier for the application.</span></span> |
|<span data-ttu-id="aacee-114">permissionIds</span><span class="sxs-lookup"><span data-stu-id="aacee-114">permissionIds</span></span>|<span data-ttu-id="aacee-115">String collection</span><span class="sxs-lookup"><span data-stu-id="aacee-115">String collection</span></span>| <span data-ttu-id="aacee-116">应用程序所需的[oauth2PermissionScopes](permissionscope.md)的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aacee-116">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="aacee-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aacee-117">JSON representation</span></span>
<span data-ttu-id="aacee-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aacee-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "permissionIds": ["String"]
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "preAuthorizedApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
