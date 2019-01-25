---
title: governanceSubject 资源类型
description: 表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519162"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="1e55a-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e55a-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e55a-104">表示用户、 组和管理特权标识管理 (PIM) 中的服务主体。</span><span class="sxs-lookup"><span data-stu-id="1e55a-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="1e55a-105">属性</span><span class="sxs-lookup"><span data-stu-id="1e55a-105">Properties</span></span>
| <span data-ttu-id="1e55a-106">属性</span><span class="sxs-lookup"><span data-stu-id="1e55a-106">Property</span></span>  | <span data-ttu-id="1e55a-107">类型</span><span class="sxs-lookup"><span data-stu-id="1e55a-107">Type</span></span>       |<span data-ttu-id="1e55a-108">说明</span><span class="sxs-lookup"><span data-stu-id="1e55a-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="1e55a-109">id</span><span class="sxs-lookup"><span data-stu-id="1e55a-109">id</span></span>         |<span data-ttu-id="1e55a-110">字串符号</span><span class="sxs-lookup"><span data-stu-id="1e55a-110">String</span></span>     | <span data-ttu-id="1e55a-111">主题的 id。</span><span class="sxs-lookup"><span data-stu-id="1e55a-111">The id of the subject.</span></span>|
|<span data-ttu-id="1e55a-112">type</span><span class="sxs-lookup"><span data-stu-id="1e55a-112">type</span></span>       |<span data-ttu-id="1e55a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="1e55a-113">String</span></span>     |<span data-ttu-id="1e55a-114">主题类型。</span><span class="sxs-lookup"><span data-stu-id="1e55a-114">The type of the subject.</span></span> <span data-ttu-id="1e55a-115">值可以是``User``， ``Group``，和``ServicePrincipal``。</span><span class="sxs-lookup"><span data-stu-id="1e55a-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="1e55a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="1e55a-116">displayName</span></span>|<span data-ttu-id="1e55a-117">String</span><span class="sxs-lookup"><span data-stu-id="1e55a-117">String</span></span>     |<span data-ttu-id="1e55a-118">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1e55a-118">The display name of the subject.</span></span>|
|<span data-ttu-id="1e55a-119">email</span><span class="sxs-lookup"><span data-stu-id="1e55a-119">email</span></span>      |<span data-ttu-id="1e55a-120">String</span><span class="sxs-lookup"><span data-stu-id="1e55a-120">String</span></span>     |<span data-ttu-id="1e55a-121">用户使用者的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="1e55a-121">The email address of the user subject.</span></span> <span data-ttu-id="1e55a-122">如果主题位于其他类型，它为空。</span><span class="sxs-lookup"><span data-stu-id="1e55a-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="1e55a-123">principalName</span><span class="sxs-lookup"><span data-stu-id="1e55a-123">principalName</span></span>|<span data-ttu-id="1e55a-124">String</span><span class="sxs-lookup"><span data-stu-id="1e55a-124">String</span></span>   |<span data-ttu-id="1e55a-125">主体的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="1e55a-125">The principal name of the user subject.</span></span> <span data-ttu-id="1e55a-126">如果主题位于其他类型，它为空。</span><span class="sxs-lookup"><span data-stu-id="1e55a-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e55a-127">关系</span><span class="sxs-lookup"><span data-stu-id="1e55a-127">Relationships</span></span>
<span data-ttu-id="1e55a-128">无</span><span class="sxs-lookup"><span data-stu-id="1e55a-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e55a-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e55a-129">JSON representation</span></span>

<span data-ttu-id="1e55a-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e55a-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
