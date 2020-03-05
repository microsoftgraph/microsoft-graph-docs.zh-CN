---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，它是使用 Azure Active Directory （Azure AD）创建和管理的。 您可以根据您的方案使用以下方法来创建和管理 Azure Active Directory 使用条款功能。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 9d45be38338554a1bf5181e4f7a3624b3d928127
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508385"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="da942-104">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="da942-104">agreement resource type</span></span>

<span data-ttu-id="da942-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="da942-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da942-106">表示租户的可自定义使用条款协议，它是使用 Azure Active Directory （Azure AD）创建和管理的。</span><span class="sxs-lookup"><span data-stu-id="da942-106">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="da942-107">您可以根据您的方案使用以下方法来创建和管理[Azure Active Directory 使用条款功能](/azure/active-directory/active-directory-tou)。</span><span class="sxs-lookup"><span data-stu-id="da942-107">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="da942-108">方法</span><span class="sxs-lookup"><span data-stu-id="da942-108">Methods</span></span>

| <span data-ttu-id="da942-109">方法</span><span class="sxs-lookup"><span data-stu-id="da942-109">Method</span></span>       | <span data-ttu-id="da942-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="da942-110">Return Type</span></span> | <span data-ttu-id="da942-111">说明</span><span class="sxs-lookup"><span data-stu-id="da942-111">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="da942-112">创建协议</span><span class="sxs-lookup"><span data-stu-id="da942-112">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="da942-113">本</span><span class="sxs-lookup"><span data-stu-id="da942-113">agreement</span></span>](agreement.md) | <span data-ttu-id="da942-114">通过发布到协议集合创建新协议。</span><span class="sxs-lookup"><span data-stu-id="da942-114">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="da942-115">列出协议</span><span class="sxs-lookup"><span data-stu-id="da942-115">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="da942-116">[协议](agreement.md)集合</span><span class="sxs-lookup"><span data-stu-id="da942-116">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="da942-117">获取一个协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="da942-117">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="da942-118">获取协议</span><span class="sxs-lookup"><span data-stu-id="da942-118">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="da942-119">本</span><span class="sxs-lookup"><span data-stu-id="da942-119">agreement</span></span>](agreement.md) | <span data-ttu-id="da942-120">读取协议对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da942-120">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="da942-121">更新协议</span><span class="sxs-lookup"><span data-stu-id="da942-121">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="da942-122">本</span><span class="sxs-lookup"><span data-stu-id="da942-122">agreement</span></span>](agreement.md) | <span data-ttu-id="da942-123">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="da942-123">Update an agreement object.</span></span> |
| [<span data-ttu-id="da942-124">删除协议</span><span class="sxs-lookup"><span data-stu-id="da942-124">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="da942-125">无</span><span class="sxs-lookup"><span data-stu-id="da942-125">None</span></span> | <span data-ttu-id="da942-126">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="da942-126">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="da942-127">属性</span><span class="sxs-lookup"><span data-stu-id="da942-127">Properties</span></span>
| <span data-ttu-id="da942-128">属性</span><span class="sxs-lookup"><span data-stu-id="da942-128">Property</span></span>     | <span data-ttu-id="da942-129">类型</span><span class="sxs-lookup"><span data-stu-id="da942-129">Type</span></span>        | <span data-ttu-id="da942-130">说明</span><span class="sxs-lookup"><span data-stu-id="da942-130">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da942-131">displayName</span><span class="sxs-lookup"><span data-stu-id="da942-131">displayName</span></span>|<span data-ttu-id="da942-132">String</span><span class="sxs-lookup"><span data-stu-id="da942-132">String</span></span>|<span data-ttu-id="da942-133">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="da942-133">Display name of the agreement.</span></span>|
|<span data-ttu-id="da942-134">id</span><span class="sxs-lookup"><span data-stu-id="da942-134">id</span></span>|<span data-ttu-id="da942-135">String</span><span class="sxs-lookup"><span data-stu-id="da942-135">String</span></span>| <span data-ttu-id="da942-136">只读。</span><span class="sxs-lookup"><span data-stu-id="da942-136">Read-only.</span></span>|
|<span data-ttu-id="da942-137">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="da942-137">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="da942-138">布尔</span><span class="sxs-lookup"><span data-stu-id="da942-138">Boolean</span></span>|<span data-ttu-id="da942-139">指示用户是否必须在接受前展开并查看协议。</span><span class="sxs-lookup"><span data-stu-id="da942-139">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da942-140">关系</span><span class="sxs-lookup"><span data-stu-id="da942-140">Relationships</span></span>
| <span data-ttu-id="da942-141">关系</span><span class="sxs-lookup"><span data-stu-id="da942-141">Relationship</span></span> | <span data-ttu-id="da942-142">类型</span><span class="sxs-lookup"><span data-stu-id="da942-142">Type</span></span>        | <span data-ttu-id="da942-143">说明</span><span class="sxs-lookup"><span data-stu-id="da942-143">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="da942-144">files</span><span class="sxs-lookup"><span data-stu-id="da942-144">files</span></span>|<span data-ttu-id="da942-145">[agreementFile](agreementfile.md)集合</span><span class="sxs-lookup"><span data-stu-id="da942-145">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="da942-146">只读。</span><span class="sxs-lookup"><span data-stu-id="da942-146">Read-only.</span></span> <span data-ttu-id="da942-147">链接到此协议的 Pdf。</span><span class="sxs-lookup"><span data-stu-id="da942-147">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="da942-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="da942-148">JSON representation</span></span>

<span data-ttu-id="da942-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da942-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "isViewingBeforeAcceptanceRequired": true
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
