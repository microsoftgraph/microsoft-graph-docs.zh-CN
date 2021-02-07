---
title: requiredResourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围的应用程序角色集。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 0ca072b679a7ec3b69c311d09aaf2000f4754f19
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133257"
---
# <a name="requiredresourceaccess-resource-type"></a><span data-ttu-id="172d6-103">requiredResourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="172d6-103">requiredResourceAccess resource type</span></span>

<span data-ttu-id="172d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="172d6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="172d6-105">指定应用程序需要访问的指定资源下的 OAuth 2.0 权限范围和应用角色集。</span><span class="sxs-lookup"><span data-stu-id="172d6-105">Specifies the set of OAuth 2.0 permission scopes and app roles under the specified resource that an application requires access to.</span></span> <span data-ttu-id="172d6-106">指定的 OAuth 2.0 权限范围可能由客户端应用程序请求 (调用资源应用程序时通过 **requiredResourceAccess**) 请求。</span><span class="sxs-lookup"><span data-stu-id="172d6-106">The specified OAuth 2.0 permission scopes may be requested by client applications (through the **requiredResourceAccess** collection) when calling a resource application.</span></span> <span data-ttu-id="172d6-107">**应用程序实体的 requiredResourceAccess** 属性是 **Re一redResourceAccess 的集合**。 [](application.md)</span><span class="sxs-lookup"><span data-stu-id="172d6-107">The **requiredResourceAccess** property of the [application](application.md) entity is a collection of **ReqiredResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="172d6-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="172d6-108">JSON representation</span></span>

<span data-ttu-id="172d6-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="172d6-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.requiredResourceAccess"
}-->

```json
{
  "resourceAccess": [{"@odata.type": "microsoft.graph.resourceAccess"}],
  "resourceAppId": "string"
}

```
## <a name="properties"></a><span data-ttu-id="172d6-110">属性</span><span class="sxs-lookup"><span data-stu-id="172d6-110">Properties</span></span>
| <span data-ttu-id="172d6-111">属性</span><span class="sxs-lookup"><span data-stu-id="172d6-111">Property</span></span>     | <span data-ttu-id="172d6-112">类型</span><span class="sxs-lookup"><span data-stu-id="172d6-112">Type</span></span>   |<span data-ttu-id="172d6-113">说明</span><span class="sxs-lookup"><span data-stu-id="172d6-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="172d6-114">resourceAccess</span><span class="sxs-lookup"><span data-stu-id="172d6-114">resourceAccess</span></span>|<span data-ttu-id="172d6-115">[resourceAccess](resourceaccess.md) 集合</span><span class="sxs-lookup"><span data-stu-id="172d6-115">[resourceAccess](resourceaccess.md) collection</span></span>|<span data-ttu-id="172d6-116">应用程序从指定资源请求的 OAuth2.0 权限范围和应用角色列表。</span><span class="sxs-lookup"><span data-stu-id="172d6-116">The list of OAuth2.0 permission scopes and app roles that the application requires from the specified resource.</span></span>|
|<span data-ttu-id="172d6-117">resourceAppId</span><span class="sxs-lookup"><span data-stu-id="172d6-117">resourceAppId</span></span>|<span data-ttu-id="172d6-118">String</span><span class="sxs-lookup"><span data-stu-id="172d6-118">String</span></span>|<span data-ttu-id="172d6-119">应用程序需要访问的资源的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="172d6-119">The unique identifier for the resource that the application requires access to.</span></span>  <span data-ttu-id="172d6-120">这应该等于在目标资源应用程序上声明的 **appId。**</span><span class="sxs-lookup"><span data-stu-id="172d6-120">This should be equal to the **appId** declared on the target resource application.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "requiredResourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

