---
title: preAuthorizedApplication 资源类型
description: 列出预授权的客户端应用程序
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 94a8dad23492ca7a145c5839410edf0fd4a34877
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761161"
---
# <a name="preauthorizedapplication-resource-type"></a><span data-ttu-id="e570f-103">preAuthorizedApplication 资源类型</span><span class="sxs-lookup"><span data-stu-id="e570f-103">preAuthorizedApplication resource type</span></span>

<span data-ttu-id="e570f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e570f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e570f-105">列出具有访问此应用程序 API 的指定权限的预授权客户端应用程序。</span><span class="sxs-lookup"><span data-stu-id="e570f-105">Lists the client applications that are pre-authorized with the specified permissions to access this application's APIs.</span></span> <span data-ttu-id="e570f-106">对于用户指定的权限，用户无需同意任何 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="e570f-106">Users are not required to consent to any pre-authorized application (for the permissions specified).</span></span> <span data-ttu-id="e570f-107">但是，未在预AuthorizedApplications中 (增量许可请求的其他权限（例如) ）将需要用户同意。</span><span class="sxs-lookup"><span data-stu-id="e570f-107">However, any additional permissions not listed in preAuthorizedApplications (requested through incremental consent for example) will require user consent.</span></span>

## <a name="properties"></a><span data-ttu-id="e570f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e570f-108">Properties</span></span>

| <span data-ttu-id="e570f-109">属性</span><span class="sxs-lookup"><span data-stu-id="e570f-109">Property</span></span> | <span data-ttu-id="e570f-110">类型</span><span class="sxs-lookup"><span data-stu-id="e570f-110">Type</span></span> | <span data-ttu-id="e570f-111">说明</span><span class="sxs-lookup"><span data-stu-id="e570f-111">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="e570f-112">appId</span><span class="sxs-lookup"><span data-stu-id="e570f-112">appId</span></span>|<span data-ttu-id="e570f-113">String</span><span class="sxs-lookup"><span data-stu-id="e570f-113">String</span></span>| <span data-ttu-id="e570f-114">应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e570f-114">The unique identifier for the application.</span></span> |
|<span data-ttu-id="e570f-115">permissionIds</span><span class="sxs-lookup"><span data-stu-id="e570f-115">permissionIds</span></span>|<span data-ttu-id="e570f-116">字符串集合</span><span class="sxs-lookup"><span data-stu-id="e570f-116">String collection</span></span>| <span data-ttu-id="e570f-117">应用程序所需的 [oauth2PermissionScopes 的唯](permissionscope.md) 一标识符。</span><span class="sxs-lookup"><span data-stu-id="e570f-117">The unique identifier for the [oauth2PermissionScopes](permissionscope.md) the application requires.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e570f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e570f-118">JSON representation</span></span>
<span data-ttu-id="e570f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e570f-119">Here is a JSON representation of the resource.</span></span>

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


