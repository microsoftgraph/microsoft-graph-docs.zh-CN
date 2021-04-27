---
title: relatedContact 资源类型
description: 与教育用户相关的联系人记录为监护人、助手、儿童等提供相关信息。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4859492f016b88a39c375d3556270f5496b8b318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035951"
---
# <a name="relatedcontact-resource-type"></a><span data-ttu-id="22d3b-103">relatedContact 资源类型</span><span class="sxs-lookup"><span data-stu-id="22d3b-103">relatedContact resource type</span></span>

<span data-ttu-id="22d3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22d3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="22d3b-105">与教育用户相关的联系人 [记录为](../resources/educationuser.md) 监护人、助手、儿童等提供相关信息。</span><span class="sxs-lookup"><span data-stu-id="22d3b-105">Contact record related to an [educationUser](../resources/educationuser.md) that provides information for guardians, aides, doctors, and so on.</span></span>

## <a name="methods"></a><span data-ttu-id="22d3b-106">方法</span><span class="sxs-lookup"><span data-stu-id="22d3b-106">Methods</span></span>

| <span data-ttu-id="22d3b-107">方法</span><span class="sxs-lookup"><span data-stu-id="22d3b-107">Method</span></span>                                    | <span data-ttu-id="22d3b-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="22d3b-108">Return Type</span></span>                   | <span data-ttu-id="22d3b-109">说明</span><span class="sxs-lookup"><span data-stu-id="22d3b-109">Description</span></span>                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [<span data-ttu-id="22d3b-110">更新</span><span class="sxs-lookup"><span data-stu-id="22d3b-110">Update</span></span>](../api/relatedcontact-update.md) | <span data-ttu-id="22d3b-111">**relatedContact** 集合</span><span class="sxs-lookup"><span data-stu-id="22d3b-111">**relatedContact** collection</span></span> | <span data-ttu-id="22d3b-112">更新[educationUser 的 relatedContacts](educationuser.md) </span><span class="sxs-lookup"><span data-stu-id="22d3b-112">Update the **relatedContacts** for an [educationUser](educationuser.md)</span></span> |

## <a name="properties"></a><span data-ttu-id="22d3b-113">属性</span><span class="sxs-lookup"><span data-stu-id="22d3b-113">Properties</span></span>

| <span data-ttu-id="22d3b-114">属性</span><span class="sxs-lookup"><span data-stu-id="22d3b-114">Property</span></span>      | <span data-ttu-id="22d3b-115">类型</span><span class="sxs-lookup"><span data-stu-id="22d3b-115">Type</span></span>                | <span data-ttu-id="22d3b-116">说明</span><span class="sxs-lookup"><span data-stu-id="22d3b-116">Description</span></span>                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="22d3b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="22d3b-117">displayName</span></span>   | <span data-ttu-id="22d3b-118">String</span><span class="sxs-lookup"><span data-stu-id="22d3b-118">String</span></span>              | <span data-ttu-id="22d3b-119">联系人的姓名。</span><span class="sxs-lookup"><span data-stu-id="22d3b-119">Name of the contact.</span></span> <span data-ttu-id="22d3b-120">必需。</span><span class="sxs-lookup"><span data-stu-id="22d3b-120">Required.</span></span>                                                                                                             |
| <span data-ttu-id="22d3b-121">accessConsent</span><span class="sxs-lookup"><span data-stu-id="22d3b-121">accessConsent</span></span> | <span data-ttu-id="22d3b-122">布尔值</span><span class="sxs-lookup"><span data-stu-id="22d3b-122">Boolean</span></span>             | <span data-ttu-id="22d3b-123">指示用户是否已同意访问学生数据。</span><span class="sxs-lookup"><span data-stu-id="22d3b-123">Indicates whether the user has been consented to access student data.</span></span>                                                                      |
| <span data-ttu-id="22d3b-124">emailAddress</span><span class="sxs-lookup"><span data-stu-id="22d3b-124">emailAddress</span></span>  | <span data-ttu-id="22d3b-125">String</span><span class="sxs-lookup"><span data-stu-id="22d3b-125">String</span></span>              | <span data-ttu-id="22d3b-126">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="22d3b-126">Email address of the contact.</span></span>                                                                                                              |
| <span data-ttu-id="22d3b-127">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="22d3b-127">mobilePhone</span></span>   | <span data-ttu-id="22d3b-128">String</span><span class="sxs-lookup"><span data-stu-id="22d3b-128">String</span></span>              | <span data-ttu-id="22d3b-129">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="22d3b-129">Mobile phone number of the contact.</span></span>                                                                                                        |
| <span data-ttu-id="22d3b-130">关系</span><span class="sxs-lookup"><span data-stu-id="22d3b-130">relationship</span></span>  | <span data-ttu-id="22d3b-131">contactRelationship</span><span class="sxs-lookup"><span data-stu-id="22d3b-131">contactRelationship</span></span> | <span data-ttu-id="22d3b-132">与用户的关系。</span><span class="sxs-lookup"><span data-stu-id="22d3b-132">Relationship to the user.</span></span> <span data-ttu-id="22d3b-133">可取值为：`parent`、`relative`、`aide`、`doctor`、`guardian`、`child`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="22d3b-133">Possible values are: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="22d3b-134">关系</span><span class="sxs-lookup"><span data-stu-id="22d3b-134">Relationships</span></span>

<span data-ttu-id="22d3b-135">无。</span><span class="sxs-lookup"><span data-stu-id="22d3b-135">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="22d3b-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22d3b-136">JSON representation</span></span>

<span data-ttu-id="22d3b-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22d3b-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
