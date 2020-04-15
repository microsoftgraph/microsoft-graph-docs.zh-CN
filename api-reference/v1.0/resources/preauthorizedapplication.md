---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 43a871eb478334f49d352ae1d56845aeef50ff03
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43474073"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="f3bd6-103">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3bd6-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="f3bd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3bd6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f3bd6-105">列出使用指定权限预授权的客户端应用程序，以访问此应用程序的 Api。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="f3bd6-106">用户无需同意任何预先授权的应用程序（针对指定的权限）。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="f3bd6-107">但是，preAuthorizedApplications 中未列出的任何其他权限（例如，通过增量许可请求）将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="f3bd6-108">属性</span><span class="sxs-lookup"><span data-stu-id="f3bd6-108">Properties</span></span>

| <span data-ttu-id="f3bd6-109">属性</span><span class="sxs-lookup"><span data-stu-id="f3bd6-109">Property</span></span> | <span data-ttu-id="f3bd6-110">类型</span><span class="sxs-lookup"><span data-stu-id="f3bd6-110">Type</span></span> | <span data-ttu-id="f3bd6-111">说明</span><span class="sxs-lookup"><span data-stu-id="f3bd6-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f3bd6-112">appId</span><span class="sxs-lookup"><span data-stu-id="f3bd6-112">appId</span></span>|<span data-ttu-id="f3bd6-113">String</span><span class="sxs-lookup"><span data-stu-id="f3bd6-113">String</span></span>| <span data-ttu-id="f3bd6-114">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="f3bd6-115">delegatedPermissionIds</span><span class="sxs-lookup"><span data-stu-id="f3bd6-115">delegatedPermissionIds</span></span>|<span data-ttu-id="f3bd6-116">String 集合</span><span class="sxs-lookup"><span data-stu-id="f3bd6-116">String collection</span></span>| <span data-ttu-id="f3bd6-117">应用程序所需的[oauth2PermissionScopes](permissionscope.md)的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f3bd6-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3bd6-118">JSON representation</span></span>
<span data-ttu-id="f3bd6-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3bd6-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.preAuthorizedApplication"
}-->

```json
{
  "appId": "String",
  "delegatedPermissionIds": ["String"]
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
