---
title: governanceSubject 资源类型
description: 表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506425"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="5453c-103">governanceSubject 资源类型</span><span class="sxs-lookup"><span data-stu-id="5453c-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5453c-104">表示在特权标识管理 (PIM) 中管理的用户、组和服务主体。</span><span class="sxs-lookup"><span data-stu-id="5453c-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="5453c-105">属性</span><span class="sxs-lookup"><span data-stu-id="5453c-105">Properties</span></span>
| <span data-ttu-id="5453c-106">属性</span><span class="sxs-lookup"><span data-stu-id="5453c-106">Property</span></span>  | <span data-ttu-id="5453c-107">类型</span><span class="sxs-lookup"><span data-stu-id="5453c-107">Type</span></span>       |<span data-ttu-id="5453c-108">说明</span><span class="sxs-lookup"><span data-stu-id="5453c-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="5453c-109">id</span><span class="sxs-lookup"><span data-stu-id="5453c-109">id</span></span>         |<span data-ttu-id="5453c-110">String</span><span class="sxs-lookup"><span data-stu-id="5453c-110">String</span></span>     | <span data-ttu-id="5453c-111">主题的 id。</span><span class="sxs-lookup"><span data-stu-id="5453c-111">The id of the subject.</span></span>|
|<span data-ttu-id="5453c-112">类型</span><span class="sxs-lookup"><span data-stu-id="5453c-112">type</span></span>       |<span data-ttu-id="5453c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="5453c-113">String</span></span>     |<span data-ttu-id="5453c-114">主题的类型。</span><span class="sxs-lookup"><span data-stu-id="5453c-114">The type of the subject.</span></span> <span data-ttu-id="5453c-115">值可以是``User``、 ``Group``和。 ``ServicePrincipal``</span><span class="sxs-lookup"><span data-stu-id="5453c-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="5453c-116">displayName</span><span class="sxs-lookup"><span data-stu-id="5453c-116">displayName</span></span>|<span data-ttu-id="5453c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="5453c-117">String</span></span>     |<span data-ttu-id="5453c-118">主题的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5453c-118">The display name of the subject.</span></span>|
|<span data-ttu-id="5453c-119">email</span><span class="sxs-lookup"><span data-stu-id="5453c-119">email</span></span>      |<span data-ttu-id="5453c-120">字符串</span><span class="sxs-lookup"><span data-stu-id="5453c-120">String</span></span>     |<span data-ttu-id="5453c-121">用户主题的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5453c-121">The email address of the user subject.</span></span> <span data-ttu-id="5453c-122">如果主题在其他类型中, 则为空。</span><span class="sxs-lookup"><span data-stu-id="5453c-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="5453c-123">principalName</span><span class="sxs-lookup"><span data-stu-id="5453c-123">principalName</span></span>|<span data-ttu-id="5453c-124">String</span><span class="sxs-lookup"><span data-stu-id="5453c-124">String</span></span>   |<span data-ttu-id="5453c-125">用户主题的主体名称。</span><span class="sxs-lookup"><span data-stu-id="5453c-125">The principal name of the user subject.</span></span> <span data-ttu-id="5453c-126">如果主题在其他类型中, 则为空。</span><span class="sxs-lookup"><span data-stu-id="5453c-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5453c-127">关系</span><span class="sxs-lookup"><span data-stu-id="5453c-127">Relationships</span></span>
<span data-ttu-id="5453c-128">无</span><span class="sxs-lookup"><span data-stu-id="5453c-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5453c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5453c-129">JSON representation</span></span>

<span data-ttu-id="5453c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5453c-130">Here is a JSON representation of the resource.</span></span>

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
