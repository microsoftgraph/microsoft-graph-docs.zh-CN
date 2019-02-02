---
title: relatedContact 资源类型
description: 联系人与提供的监护人、 工具、 医生，等信息 educationUser 相关的记录。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: d29cf93154e2c032ac7010372e3f116f2a1dd46c
ms.sourcegitcommit: d6209114cbbe8072e3ecf7eba23819ae5ace7db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/01/2019
ms.locfileid: "29694473"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="7db6a-103">relatedContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="7db6a-103">relatedContact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7db6a-104">联系人提供监护人、 工具、 医生，等 inforation [educationUser](../resources/educationuser.md)与相关的记录。</span><span class="sxs-lookup"><span data-stu-id="7db6a-104">Contact record related to an [educationUser](../resources/educationuser.md) that provides inforation for guardians, aides, doctors, and so on.</span></span>

## <a name="properties"></a><span data-ttu-id="7db6a-105">属性</span><span class="sxs-lookup"><span data-stu-id="7db6a-105">Properties</span></span>
| <span data-ttu-id="7db6a-106">属性</span><span class="sxs-lookup"><span data-stu-id="7db6a-106">Property</span></span>     | <span data-ttu-id="7db6a-107">类型</span><span class="sxs-lookup"><span data-stu-id="7db6a-107">Type</span></span>   |<span data-ttu-id="7db6a-108">说明</span><span class="sxs-lookup"><span data-stu-id="7db6a-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7db6a-109">id</span><span class="sxs-lookup"><span data-stu-id="7db6a-109">id</span></span>|<span data-ttu-id="7db6a-110">字符串</span><span class="sxs-lookup"><span data-stu-id="7db6a-110">String</span></span>|<span data-ttu-id="7db6a-111">在 Azure Active Directory 联系人的标识。</span><span class="sxs-lookup"><span data-stu-id="7db6a-111">Identity of the contact within Azure Active Directory.</span></span>|
|<span data-ttu-id="7db6a-112">displayName</span><span class="sxs-lookup"><span data-stu-id="7db6a-112">displayName</span></span>|<span data-ttu-id="7db6a-113">字符串</span><span class="sxs-lookup"><span data-stu-id="7db6a-113">String</span></span>|<span data-ttu-id="7db6a-114">联系人的姓名。</span><span class="sxs-lookup"><span data-stu-id="7db6a-114">Name of the contact.</span></span> <span data-ttu-id="7db6a-115">必需。</span><span class="sxs-lookup"><span data-stu-id="7db6a-115">Required.</span></span>|
|<span data-ttu-id="7db6a-116">emailAddress</span><span class="sxs-lookup"><span data-stu-id="7db6a-116">emailAddress</span></span>|<span data-ttu-id="7db6a-117">String</span><span class="sxs-lookup"><span data-stu-id="7db6a-117">String</span></span>|<span data-ttu-id="7db6a-118">该联系人的主电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="7db6a-118">Primary email address of the contact.</span></span>|
|<span data-ttu-id="7db6a-119">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="7db6a-119">mobilePhone</span></span>|<span data-ttu-id="7db6a-120">字符串</span><span class="sxs-lookup"><span data-stu-id="7db6a-120">String</span></span>|<span data-ttu-id="7db6a-121">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="7db6a-121">Mobile phone number of the contact.</span></span>|
|<span data-ttu-id="7db6a-122">关系</span><span class="sxs-lookup"><span data-stu-id="7db6a-122">relationship</span></span>|`contactRelationship`|<span data-ttu-id="7db6a-123">向用户的关系。</span><span class="sxs-lookup"><span data-stu-id="7db6a-123">Relationship to the user.</span></span> <span data-ttu-id="7db6a-124">可能的值为`parent`， `relative`， `aide`， `doctor`， `guardian`， `child`， `other`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="7db6a-124">Possible values are `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="7db6a-125">accessConsent</span><span class="sxs-lookup"><span data-stu-id="7db6a-125">accessConsent</span></span>|<span data-ttu-id="7db6a-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="7db6a-126">Boolean</span></span>|<span data-ttu-id="7db6a-127">指示是否用户具有已同意访问学生数据。</span><span class="sxs-lookup"><span data-stu-id="7db6a-127">Indicates whether the user has been consented to access student data.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7db6a-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7db6a-128">JSON representation</span></span>

<span data-ttu-id="7db6a-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7db6a-129">The following is a JSON representation of the resource.</span></span>

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
