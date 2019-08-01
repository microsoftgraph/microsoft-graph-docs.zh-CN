---
title: relatedContact 资源类型
description: 与为监护人、工具、医生等提供信息的 educationUser 相关的联系人记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 7a2040bbe357a7cc89dffed1ad4332bf89077204
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034760"
---
# <a name="realtedcontact-resource-type"></a><span data-ttu-id="0b8bb-103">realtedContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="0b8bb-103">realtedContact resource type</span></span>

<span data-ttu-id="0b8bb-104">与为监护人、工具、医生等提供信息的[educationUser](../resources/educationuser.md)相关的联系人记录。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="0b8bb-105">属性</span><span class="sxs-lookup"><span data-stu-id="0b8bb-105">Properties</span></span>
| <span data-ttu-id="0b8bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="0b8bb-106">Property</span></span>     | <span data-ttu-id="0b8bb-107">类型</span><span class="sxs-lookup"><span data-stu-id="0b8bb-107">Type</span></span>   |<span data-ttu-id="0b8bb-108">说明</span><span class="sxs-lookup"><span data-stu-id="0b8bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0b8bb-109">id</span><span class="sxs-lookup"><span data-stu-id="0b8bb-109">id</span></span>|<span data-ttu-id="0b8bb-110">字符串</span><span class="sxs-lookup"><span data-stu-id="0b8bb-110">String</span></span>|<span data-ttu-id="0b8bb-111">Azure Active Directory 中的联系人的标识。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="0b8bb-112">displayName</span><span class="sxs-lookup"><span data-stu-id="0b8bb-112">displayName</span></span>|<span data-ttu-id="0b8bb-113">字符串</span><span class="sxs-lookup"><span data-stu-id="0b8bb-113">String</span></span>|<span data-ttu-id="0b8bb-114">联系人的名称。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-114">Name of the contact.</span></span> <span data-ttu-id="0b8bb-115">必需。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-115">Required.</span></span>|
|<span data-ttu-id="0b8bb-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="0b8bb-116">emailAddress</span></span>|<span data-ttu-id="0b8bb-117">String</span><span class="sxs-lookup"><span data-stu-id="0b8bb-117">String</span></span>|<span data-ttu-id="0b8bb-118">联系人的主电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="0b8bb-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="0b8bb-119">mobilePhone</span></span>|<span data-ttu-id="0b8bb-120">String</span><span class="sxs-lookup"><span data-stu-id="0b8bb-120">String</span></span>|<span data-ttu-id="0b8bb-121">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="0b8bb-122">关系</span><span class="sxs-lookup"><span data-stu-id="0b8bb-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="0b8bb-123">与用户的关系。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-123">Relationship to the user.</span></span> <span data-ttu-id="0b8bb-124">可能的值`parent`为`relative`、 `aide` `doctor` `guardian` `child`、、、、、 `unknownFutureValue` `other`</span><span class="sxs-lookup"><span data-stu-id="0b8bb-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0b8bb-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="0b8bb-125">accessConsent</span></span>|<span data-ttu-id="0b8bb-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b8bb-126">Boolean</span></span>|<span data-ttu-id="0b8bb-127">指示用户是否同意访问学生数据。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0b8bb-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0b8bb-128">JSON representation</span></span>

<span data-ttu-id="0b8bb-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b8bb-129">The following is a JSON representation of the resource.</span></span>

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
