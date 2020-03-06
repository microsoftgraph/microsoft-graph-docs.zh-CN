---
title: relatedContact 资源类型
description: 与为监护人、工具、医生等提供信息的 educationUser 相关的联系人记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 93069c2f9f2aa46c5d6d0f2f992762efab062064
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533860"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="0bfca-103">realtedContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="0bfca-103">realtedContact resource type</span></span>

<span data-ttu-id="0bfca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0bfca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0bfca-105">与为监护人、工具、医生等提供信息的[educationUser](../resources/educationuser.md)相关的联系人记录。</span><span class="sxs-lookup"><span data-stu-id="0bfca-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="0bfca-106">属性</span><span class="sxs-lookup"><span data-stu-id="0bfca-106">Properties</span></span>
| <span data-ttu-id="0bfca-107">属性</span><span class="sxs-lookup"><span data-stu-id="0bfca-107">Property</span></span>     | <span data-ttu-id="0bfca-108">类型</span><span class="sxs-lookup"><span data-stu-id="0bfca-108">Type</span></span>   |<span data-ttu-id="0bfca-109">说明</span><span class="sxs-lookup"><span data-stu-id="0bfca-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0bfca-110">id</span><span class="sxs-lookup"><span data-stu-id="0bfca-110">id</span></span>|<span data-ttu-id="0bfca-111">字符串</span><span class="sxs-lookup"><span data-stu-id="0bfca-111">String</span></span>|<span data-ttu-id="0bfca-112">Azure Active Directory 中的联系人的标识。</span><span class="sxs-lookup"><span data-stu-id="0bfca-112">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="0bfca-113">displayName</span><span class="sxs-lookup"><span data-stu-id="0bfca-113">displayName</span></span>|<span data-ttu-id="0bfca-114">字符串</span><span class="sxs-lookup"><span data-stu-id="0bfca-114">String</span></span>|<span data-ttu-id="0bfca-115">联系人的名称。</span><span class="sxs-lookup"><span data-stu-id="0bfca-115">Name of the contact.</span></span> <span data-ttu-id="0bfca-116">必需。</span><span class="sxs-lookup"><span data-stu-id="0bfca-116">Required.</span></span>|
|<span data-ttu-id="0bfca-117">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0bfca-117">emailAddress</span></span>|<span data-ttu-id="0bfca-118">String</span><span class="sxs-lookup"><span data-stu-id="0bfca-118">String</span></span>|<span data-ttu-id="0bfca-119">联系人的主电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0bfca-119">Primary email address of the contact.</span></span>|
|<span data-ttu-id="0bfca-120">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0bfca-120">mobilePhone</span></span>|<span data-ttu-id="0bfca-121">String</span><span class="sxs-lookup"><span data-stu-id="0bfca-121">String</span></span>|<span data-ttu-id="0bfca-122">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="0bfca-122">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="0bfca-123">关系</span><span class="sxs-lookup"><span data-stu-id="0bfca-123">relationship</span></span>|`contactRelationship`|<span data-ttu-id="0bfca-124">与用户的关系。</span><span class="sxs-lookup"><span data-stu-id="0bfca-124">Relationship to the user.</span></span> <span data-ttu-id="0bfca-125">可能的值`parent`为`relative`、 `aide` `doctor` `guardian` `child`、、、、、 `unknownFutureValue` `other`</span><span class="sxs-lookup"><span data-stu-id="0bfca-125">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0bfca-126">accessConsent</span><span class="sxs-lookup"><span data-stu-id="0bfca-126">accessConsent</span></span>|<span data-ttu-id="0bfca-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="0bfca-127">Boolean</span></span>|<span data-ttu-id="0bfca-128">指示用户是否同意访问学生数据。</span><span class="sxs-lookup"><span data-stu-id="0bfca-128">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0bfca-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0bfca-129">JSON representation</span></span>

<span data-ttu-id="0bfca-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0bfca-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.relatedContact"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "contactRelationship",
  "accessConsent": true
}
```

<!-- uuid: 720F9AB6-6E7A-4A66-8B0A-37A556FF99C5
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "relatedContact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
