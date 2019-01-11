---
title: 协议资源类型
description: 表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。 可以使用以下方法来创建和管理 Azure Active Directory 使用条款的功能，根据您的方案。
localization_priority: Normal
ms.openlocfilehash: 8c082ed6229b44cc3a3d4cba6dd8645feee5d07c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27845344"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="2861c-104">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="2861c-104">agreement resource type</span></span>

> <span data-ttu-id="2861c-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2861c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2861c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2861c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2861c-107">表示一个租户的可自定义的创建和管理与 Azure Active Directory (Azure AD) 使用协议条款。</span><span class="sxs-lookup"><span data-stu-id="2861c-107">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="2861c-108">可以使用以下方法来创建和管理[Azure Active Directory 使用条款的功能](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou)，根据您的方案。</span><span class="sxs-lookup"><span data-stu-id="2861c-108">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="2861c-109">方法</span><span class="sxs-lookup"><span data-stu-id="2861c-109">Methods</span></span>

| <span data-ttu-id="2861c-110">方法</span><span class="sxs-lookup"><span data-stu-id="2861c-110">Method</span></span>       | <span data-ttu-id="2861c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="2861c-111">Return Type</span></span> | <span data-ttu-id="2861c-112">说明</span><span class="sxs-lookup"><span data-stu-id="2861c-112">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="2861c-113">创建协议</span><span class="sxs-lookup"><span data-stu-id="2861c-113">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="2861c-114">协议</span><span class="sxs-lookup"><span data-stu-id="2861c-114">agreement</span></span>](agreement.md) | <span data-ttu-id="2861c-115">通过发布到协议集合中创建新的协议。</span><span class="sxs-lookup"><span data-stu-id="2861c-115">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="2861c-116">列表协议</span><span class="sxs-lookup"><span data-stu-id="2861c-116">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="2861c-117">[协议](agreement.md)集合</span><span class="sxs-lookup"><span data-stu-id="2861c-117">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="2861c-118">获取协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="2861c-118">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="2861c-119">获取协议</span><span class="sxs-lookup"><span data-stu-id="2861c-119">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="2861c-120">协议</span><span class="sxs-lookup"><span data-stu-id="2861c-120">agreement</span></span>](agreement.md) | <span data-ttu-id="2861c-121">读取属性和协议对象的关系。</span><span class="sxs-lookup"><span data-stu-id="2861c-121">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="2861c-122">更新协议</span><span class="sxs-lookup"><span data-stu-id="2861c-122">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="2861c-123">协议</span><span class="sxs-lookup"><span data-stu-id="2861c-123">agreement</span></span>](agreement.md) | <span data-ttu-id="2861c-124">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="2861c-124">Update an agreement object.</span></span> |
| [<span data-ttu-id="2861c-125">删除协议</span><span class="sxs-lookup"><span data-stu-id="2861c-125">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="2861c-126">无</span><span class="sxs-lookup"><span data-stu-id="2861c-126">None</span></span> | <span data-ttu-id="2861c-127">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="2861c-127">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="2861c-128">属性</span><span class="sxs-lookup"><span data-stu-id="2861c-128">Properties</span></span>
| <span data-ttu-id="2861c-129">属性</span><span class="sxs-lookup"><span data-stu-id="2861c-129">Property</span></span>     | <span data-ttu-id="2861c-130">类型</span><span class="sxs-lookup"><span data-stu-id="2861c-130">Type</span></span>        | <span data-ttu-id="2861c-131">说明</span><span class="sxs-lookup"><span data-stu-id="2861c-131">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2861c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="2861c-132">displayName</span></span>|<span data-ttu-id="2861c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2861c-133">String</span></span>|<span data-ttu-id="2861c-134">协议中的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2861c-134">Display name of the agreement.</span></span>|
|<span data-ttu-id="2861c-135">id</span><span class="sxs-lookup"><span data-stu-id="2861c-135">id</span></span>|<span data-ttu-id="2861c-136">String</span><span class="sxs-lookup"><span data-stu-id="2861c-136">String</span></span>| <span data-ttu-id="2861c-137">只读。</span><span class="sxs-lookup"><span data-stu-id="2861c-137">Read-only.</span></span>|
|<span data-ttu-id="2861c-138">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="2861c-138">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="2861c-139">布尔</span><span class="sxs-lookup"><span data-stu-id="2861c-139">Boolean</span></span>|<span data-ttu-id="2861c-140">指示用户是否能够展开和查看接受之前协议。</span><span class="sxs-lookup"><span data-stu-id="2861c-140">Indicates whether the user has to expand and view the agreement before accepting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2861c-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="2861c-141">Relationships</span></span>
| <span data-ttu-id="2861c-142">关系</span><span class="sxs-lookup"><span data-stu-id="2861c-142">Relationship</span></span> | <span data-ttu-id="2861c-143">类型</span><span class="sxs-lookup"><span data-stu-id="2861c-143">Type</span></span>        | <span data-ttu-id="2861c-144">说明</span><span class="sxs-lookup"><span data-stu-id="2861c-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2861c-145">files</span><span class="sxs-lookup"><span data-stu-id="2861c-145">files</span></span>|<span data-ttu-id="2861c-146">[agreementFile](agreementfile.md)集合</span><span class="sxs-lookup"><span data-stu-id="2861c-146">[agreementFile](agreementfile.md) collection</span></span>|<span data-ttu-id="2861c-147">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="2861c-147">Read-only.</span></span> <span data-ttu-id="2861c-148">Pdf 链接到此协议。</span><span class="sxs-lookup"><span data-stu-id="2861c-148">PDFs linked to this agreement.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2861c-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2861c-149">JSON representation</span></span>

<span data-ttu-id="2861c-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2861c-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "agreement resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
