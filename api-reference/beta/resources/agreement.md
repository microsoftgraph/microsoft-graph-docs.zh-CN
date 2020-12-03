---
title: 协议资源类型
description: 表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 创建和管理的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 8b5b400bea6ae4435e1aa525012b7b3224a95abc
ms.sourcegitcommit: d09d720b56ed6f1fad556e2a3730c2e850db355f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/02/2020
ms.locfileid: "49555639"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="1da47-103">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="1da47-103">agreement resource type</span></span>

<span data-ttu-id="1da47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1da47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1da47-105">表示租户的可自定义使用条款协议，该协议是使用 Azure Active Directory (Azure AD) 创建和管理的。</span><span class="sxs-lookup"><span data-stu-id="1da47-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="1da47-106">您可以根据您的方案使用以下方法来创建和管理 [Azure Active Directory 使用条款功能](/azure/active-directory/active-directory-tou) 。</span><span class="sxs-lookup"><span data-stu-id="1da47-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="1da47-107">方法</span><span class="sxs-lookup"><span data-stu-id="1da47-107">Methods</span></span>

| <span data-ttu-id="1da47-108">方法</span><span class="sxs-lookup"><span data-stu-id="1da47-108">Method</span></span>       | <span data-ttu-id="1da47-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1da47-109">Return Type</span></span> | <span data-ttu-id="1da47-110">说明</span><span class="sxs-lookup"><span data-stu-id="1da47-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="1da47-111">创建协议</span><span class="sxs-lookup"><span data-stu-id="1da47-111">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="1da47-112">本</span><span class="sxs-lookup"><span data-stu-id="1da47-112">agreement</span></span>](agreement.md) | <span data-ttu-id="1da47-113">通过发布到协议集合创建新协议。</span><span class="sxs-lookup"><span data-stu-id="1da47-113">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="1da47-114">列出协议</span><span class="sxs-lookup"><span data-stu-id="1da47-114">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="1da47-115">[协议](agreement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1da47-115">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="1da47-116">获取一个协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="1da47-116">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="1da47-117">获取协议</span><span class="sxs-lookup"><span data-stu-id="1da47-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="1da47-118">本</span><span class="sxs-lookup"><span data-stu-id="1da47-118">agreement</span></span>](agreement.md) | <span data-ttu-id="1da47-119">读取协议对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1da47-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="1da47-120">更新协议</span><span class="sxs-lookup"><span data-stu-id="1da47-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="1da47-121">本</span><span class="sxs-lookup"><span data-stu-id="1da47-121">agreement</span></span>](agreement.md) | <span data-ttu-id="1da47-122">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="1da47-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="1da47-123">删除协议</span><span class="sxs-lookup"><span data-stu-id="1da47-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="1da47-124">无</span><span class="sxs-lookup"><span data-stu-id="1da47-124">None</span></span> | <span data-ttu-id="1da47-125">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="1da47-125">Delete an agreement object.</span></span> |
<!--
| [Create agreementFile](../api/agreement-post-files.md) | [agreementFile](agreementfile.md) | Create a new agreementFile by posting to the files collection. |
| [List files](../api/agreement-list-files.md) | [agreementFile](agreementfile.md) collection | Get an agreementFile object collection. |
-->

## <a name="properties"></a><span data-ttu-id="1da47-126">属性</span><span class="sxs-lookup"><span data-stu-id="1da47-126">Properties</span></span>
| <span data-ttu-id="1da47-127">属性</span><span class="sxs-lookup"><span data-stu-id="1da47-127">Property</span></span>     | <span data-ttu-id="1da47-128">类型</span><span class="sxs-lookup"><span data-stu-id="1da47-128">Type</span></span>        | <span data-ttu-id="1da47-129">说明</span><span class="sxs-lookup"><span data-stu-id="1da47-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1da47-130">displayName</span><span class="sxs-lookup"><span data-stu-id="1da47-130">displayName</span></span>|<span data-ttu-id="1da47-131">String</span><span class="sxs-lookup"><span data-stu-id="1da47-131">String</span></span>|<span data-ttu-id="1da47-132">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1da47-132">Display name of the agreement.</span></span> <span data-ttu-id="1da47-133">显示名称用于协议的内部跟踪，但不向查看该协议的最终用户显示。</span><span class="sxs-lookup"><span data-stu-id="1da47-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="1da47-134">id</span><span class="sxs-lookup"><span data-stu-id="1da47-134">id</span></span>|<span data-ttu-id="1da47-135">String</span><span class="sxs-lookup"><span data-stu-id="1da47-135">String</span></span>| <span data-ttu-id="1da47-136">只读。</span><span class="sxs-lookup"><span data-stu-id="1da47-136">Read-only.</span></span>|
|<span data-ttu-id="1da47-137">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="1da47-137">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="1da47-138">布尔值</span><span class="sxs-lookup"><span data-stu-id="1da47-138">Boolean</span></span>|<span data-ttu-id="1da47-139">通过此设置，您可以要求最终用户在其访问它的每台设备上接受此协议。</span><span class="sxs-lookup"><span data-stu-id="1da47-139">This setting enables you to require end users to accept this agreement on every device that they are accessing it from.</span></span> <span data-ttu-id="1da47-140">最终用户将需要在 Azure AD 中注册其设备（如果尚未这样做）。</span><span class="sxs-lookup"><span data-stu-id="1da47-140">The end user will be required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="1da47-141">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="1da47-141">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="1da47-142">布尔值</span><span class="sxs-lookup"><span data-stu-id="1da47-142">Boolean</span></span>|<span data-ttu-id="1da47-143">指示用户是否必须在接受前展开协议。</span><span class="sxs-lookup"><span data-stu-id="1da47-143">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="1da47-144">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="1da47-144">termsExpiration</span></span>|[<span data-ttu-id="1da47-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="1da47-145">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="1da47-146">所有用户的到期计划和协议频率。</span><span class="sxs-lookup"><span data-stu-id="1da47-146">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="1da47-147">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="1da47-147">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="1da47-148">持续时间</span><span class="sxs-lookup"><span data-stu-id="1da47-148">Duration</span></span>|<span data-ttu-id="1da47-149">持续时间，用户必须重新接受使用条款。</span><span class="sxs-lookup"><span data-stu-id="1da47-149">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="1da47-150">值以 ISO 8601 格式表示，持续时间。</span><span class="sxs-lookup"><span data-stu-id="1da47-150">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="1da47-151">关系</span><span class="sxs-lookup"><span data-stu-id="1da47-151">Relationships</span></span>
| <span data-ttu-id="1da47-152">关系</span><span class="sxs-lookup"><span data-stu-id="1da47-152">Relationship</span></span> | <span data-ttu-id="1da47-153">类型</span><span class="sxs-lookup"><span data-stu-id="1da47-153">Type</span></span>        | <span data-ttu-id="1da47-154">说明</span><span class="sxs-lookup"><span data-stu-id="1da47-154">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1da47-155">acceptances</span><span class="sxs-lookup"><span data-stu-id="1da47-155">acceptances</span></span>|<span data-ttu-id="1da47-156">[agreementAcceptance](agreementacceptance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1da47-156">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="1da47-157">只读。</span><span class="sxs-lookup"><span data-stu-id="1da47-157">Read-only.</span></span> <span data-ttu-id="1da47-158">本协议 acceptances 的相关信息。</span><span class="sxs-lookup"><span data-stu-id="1da47-158">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="1da47-159">files</span><span class="sxs-lookup"><span data-stu-id="1da47-159">files</span></span>|<span data-ttu-id="1da47-160">[agreementFileLocalization](agreementfilelocalization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1da47-160">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="1da47-161">链接到此协议的 Pdf。</span><span class="sxs-lookup"><span data-stu-id="1da47-161">PDFs linked to this agreement.</span></span> <span data-ttu-id="1da47-162">**注意：** 此属性正处于弃用的过程中。</span><span class="sxs-lookup"><span data-stu-id="1da47-162">**Note:** This property is in the process of being deprecated.</span></span> <span data-ttu-id="1da47-163">请改为使用  **file** 属性。</span><span class="sxs-lookup"><span data-stu-id="1da47-163">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="1da47-164">file</span><span class="sxs-lookup"><span data-stu-id="1da47-164">file</span></span>|[<span data-ttu-id="1da47-165">agreementFile</span><span class="sxs-lookup"><span data-stu-id="1da47-165">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="1da47-166">链接到此协议的默认 PDF。</span><span class="sxs-lookup"><span data-stu-id="1da47-166">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="1da47-167">file/localizations</span><span class="sxs-lookup"><span data-stu-id="1da47-167">file/localizations</span></span>|<span data-ttu-id="1da47-168">[agreementFileLocalization](agreementfilelocalization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1da47-168">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="1da47-169">附加到协议的协议文件的本地化版本。</span><span class="sxs-lookup"><span data-stu-id="1da47-169">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="1da47-170">file/localizations/{localizationId}/版本</span><span class="sxs-lookup"><span data-stu-id="1da47-170">file/localizations/{localizationId}/versions</span></span>|<span data-ttu-id="1da47-171">[agreementFileVersion](agreementfileversion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1da47-171">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="1da47-172">本地化协议文件的版本历史记录。</span><span class="sxs-lookup"><span data-stu-id="1da47-172">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="1da47-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1da47-173">JSON representation</span></span>

<span data-ttu-id="1da47-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1da47-174">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreement"
}-->

```json
{
  "id": "String (identifier)",
  "displayName": "MSGraph Sample",
  "isViewingBeforeAcceptanceRequired": true,
  "isPerDeviceAcceptanceRequired": false,
  "termsExpiration": {
    "startDateTime": "2018-10-01T00:00:00.0000000Z",
    "frequency": "PT1M"
  }
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


