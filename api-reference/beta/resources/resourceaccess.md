---
title: resourceAccess 资源类型
description: 指定 OAuth 2.0 权限范围或应用程序需要应用程序角色。 RequiredResourceAccess 类型的**resourceAccess**属性是**ResourceAccess**的集合。
ms.openlocfilehash: 56e9b2b006d63d2a9abebc9e9585744b08438800
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046865"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="5a87e-104">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a87e-104">resourceAccess resource type</span></span>

> <span data-ttu-id="5a87e-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5a87e-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5a87e-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5a87e-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5a87e-107">指定 OAuth 2.0 权限范围或应用程序需要应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="5a87e-107">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="5a87e-108">[RequiredResourceAccess](requiredresourceaccess.md)类型的**resourceAccess**属性是**ResourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="5a87e-108">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="5a87e-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a87e-109">JSON representation</span></span>

<span data-ttu-id="5a87e-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a87e-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.resourceAccess"
}-->

```json
{
  "id": "guid",
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="5a87e-111">属性</span><span class="sxs-lookup"><span data-stu-id="5a87e-111">Properties</span></span>
| <span data-ttu-id="5a87e-112">属性</span><span class="sxs-lookup"><span data-stu-id="5a87e-112">Property</span></span>     | <span data-ttu-id="5a87e-113">类型</span><span class="sxs-lookup"><span data-stu-id="5a87e-113">Type</span></span>   |<span data-ttu-id="5a87e-114">说明</span><span class="sxs-lookup"><span data-stu-id="5a87e-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5a87e-115">ID</span><span class="sxs-lookup"><span data-stu-id="5a87e-115">id</span></span>|<span data-ttu-id="5a87e-116">Guid</span><span class="sxs-lookup"><span data-stu-id="5a87e-116">Guid</span></span>|<span data-ttu-id="5a87e-117">一个资源应用程序公开[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)实例的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5a87e-117">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="5a87e-118">type</span><span class="sxs-lookup"><span data-stu-id="5a87e-118">type</span></span>|<span data-ttu-id="5a87e-119">字符串</span><span class="sxs-lookup"><span data-stu-id="5a87e-119">String</span></span>|<span data-ttu-id="5a87e-120">指定的**id**属性引用[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="5a87e-120">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="5a87e-121">可能的值为"作用域"或"角色"。</span><span class="sxs-lookup"><span data-stu-id="5a87e-121">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
