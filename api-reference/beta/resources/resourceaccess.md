---
title: resourceAccess 资源类型
description: 指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。 requiredResourceAccess 类型的**resourceAccess**属性是**resourceAccess**的集合。
localization_priority: Normal
ms.openlocfilehash: 1e741aa49e56b304c265a5fd701fdac37feb29dd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563038"
---
# <a name="resourceaccess-resource-type"></a><span data-ttu-id="11802-104">resourceAccess 资源类型</span><span class="sxs-lookup"><span data-stu-id="11802-104">resourceAccess resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11802-105">指定应用程序所需的 OAuth 2.0 权限范围或应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="11802-105">Specifies an OAuth 2.0 permission scope or an app role that an application requires.</span></span> <span data-ttu-id="11802-106">[requiredResourceAccess](requiredresourceaccess.md)类型的**resourceAccess**属性是**resourceAccess**的集合。</span><span class="sxs-lookup"><span data-stu-id="11802-106">The **resourceAccess** property of the [requiredResourceAccess](requiredresourceaccess.md) type is a collection of **ResourceAccess**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="11802-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11802-107">JSON representation</span></span>

<span data-ttu-id="11802-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11802-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="11802-109">属性</span><span class="sxs-lookup"><span data-stu-id="11802-109">Properties</span></span>
| <span data-ttu-id="11802-110">属性</span><span class="sxs-lookup"><span data-stu-id="11802-110">Property</span></span>     | <span data-ttu-id="11802-111">类型</span><span class="sxs-lookup"><span data-stu-id="11802-111">Type</span></span>   |<span data-ttu-id="11802-112">说明</span><span class="sxs-lookup"><span data-stu-id="11802-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="11802-113">id</span><span class="sxs-lookup"><span data-stu-id="11802-113">id</span></span>|<span data-ttu-id="11802-114">Guid</span><span class="sxs-lookup"><span data-stu-id="11802-114">Guid</span></span>|<span data-ttu-id="11802-115">资源应用程序公开的[oAuth2Permission](oauth2permission.md)或[appRole](approle.md)实例之一的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="11802-115">The unique identifier for one of the [oAuth2Permission](oauth2permission.md) or [appRole](approle.md) instances that the resource application exposes.</span></span>|
|<span data-ttu-id="11802-116">type</span><span class="sxs-lookup"><span data-stu-id="11802-116">type</span></span>|<span data-ttu-id="11802-117">String</span><span class="sxs-lookup"><span data-stu-id="11802-117">String</span></span>|<span data-ttu-id="11802-118">指定**id**属性引用的是[oAuth2Permission](oauth2permission.md)还是[appRole](approle.md)。</span><span class="sxs-lookup"><span data-stu-id="11802-118">Specifies whether the **id** property references an [oAuth2Permission](oauth2permission.md) or an [appRole](approle.md).</span></span> <span data-ttu-id="11802-119">可能的值为 "scope" 或 "role"。</span><span class="sxs-lookup"><span data-stu-id="11802-119">Possible values are "scope" or "role".</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resourceAccess resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resourceaccess.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
