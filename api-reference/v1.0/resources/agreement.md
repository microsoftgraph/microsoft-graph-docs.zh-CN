---
title: 协议资源类型
description: 表示使用 Azure AD (Azure Active Directory 创建和管理的租户可自定义) 。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: 045d4b9142d4bd0c4bc01392975871e0253d33c0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722620"
---
# <a name="agreement-resource-type"></a><span data-ttu-id="f927e-103">协议资源类型</span><span class="sxs-lookup"><span data-stu-id="f927e-103">agreement resource type</span></span>

<span data-ttu-id="f927e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f927e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f927e-105">表示使用 Azure AD (Azure Active Directory 创建和管理的租户可自定义) 。</span><span class="sxs-lookup"><span data-stu-id="f927e-105">Represents a tenant's customizable terms of use agreement that is created and managed with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="f927e-106">可以使用以下方法根据你的方案创建和管理 Azure [Active Directory](/azure/active-directory/active-directory-tou) 使用条款功能。</span><span class="sxs-lookup"><span data-stu-id="f927e-106">You can use the following methods to create and manage the [Azure Active Directory Terms of Use feature](/azure/active-directory/active-directory-tou) according to your scenario.</span></span>

## <a name="methods"></a><span data-ttu-id="f927e-107">Methods</span><span class="sxs-lookup"><span data-stu-id="f927e-107">Methods</span></span>

| <span data-ttu-id="f927e-108">方法</span><span class="sxs-lookup"><span data-stu-id="f927e-108">Method</span></span>       | <span data-ttu-id="f927e-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="f927e-109">Return Type</span></span> | <span data-ttu-id="f927e-110">说明</span><span class="sxs-lookup"><span data-stu-id="f927e-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f927e-111">列出协议</span><span class="sxs-lookup"><span data-stu-id="f927e-111">List agreements</span></span>](../api/agreement-list.md) | <span data-ttu-id="f927e-112">[协议](agreement.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f927e-112">[agreement](agreement.md) collection</span></span> | <span data-ttu-id="f927e-113">获取协议对象集合。</span><span class="sxs-lookup"><span data-stu-id="f927e-113">Get an agreement object collection.</span></span> |
| [<span data-ttu-id="f927e-114">创建协议</span><span class="sxs-lookup"><span data-stu-id="f927e-114">Create agreements</span></span>](../api/agreement-post-agreements.md) | [<span data-ttu-id="f927e-115">协议</span><span class="sxs-lookup"><span data-stu-id="f927e-115">agreement</span></span>](agreement.md) | <span data-ttu-id="f927e-116">通过发布到协议集合创建新协议。</span><span class="sxs-lookup"><span data-stu-id="f927e-116">Create a new agreement by posting to the agreement collection.</span></span> |
| [<span data-ttu-id="f927e-117">获取协议</span><span class="sxs-lookup"><span data-stu-id="f927e-117">Get agreement</span></span>](../api/agreement-get.md) | [<span data-ttu-id="f927e-118">协议</span><span class="sxs-lookup"><span data-stu-id="f927e-118">agreement</span></span>](agreement.md) | <span data-ttu-id="f927e-119">读取协议对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f927e-119">Read properties and relationships of an agreement object.</span></span> |
| [<span data-ttu-id="f927e-120">更新协议</span><span class="sxs-lookup"><span data-stu-id="f927e-120">Update agreement</span></span>](../api/agreement-update.md) | [<span data-ttu-id="f927e-121">协议</span><span class="sxs-lookup"><span data-stu-id="f927e-121">agreement</span></span>](agreement.md) | <span data-ttu-id="f927e-122">更新协议对象。</span><span class="sxs-lookup"><span data-stu-id="f927e-122">Update an agreement object.</span></span> |
| [<span data-ttu-id="f927e-123">删除协议</span><span class="sxs-lookup"><span data-stu-id="f927e-123">Delete agreement</span></span>](../api/agreement-delete.md) | <span data-ttu-id="f927e-124">无</span><span class="sxs-lookup"><span data-stu-id="f927e-124">None</span></span> | <span data-ttu-id="f927e-125">删除协议对象。</span><span class="sxs-lookup"><span data-stu-id="f927e-125">Delete an agreement object.</span></span> |

## <a name="properties"></a><span data-ttu-id="f927e-126">属性</span><span class="sxs-lookup"><span data-stu-id="f927e-126">Properties</span></span>
| <span data-ttu-id="f927e-127">属性</span><span class="sxs-lookup"><span data-stu-id="f927e-127">Property</span></span>     | <span data-ttu-id="f927e-128">类型</span><span class="sxs-lookup"><span data-stu-id="f927e-128">Type</span></span>        | <span data-ttu-id="f927e-129">说明</span><span class="sxs-lookup"><span data-stu-id="f927e-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f927e-130">displayName</span><span class="sxs-lookup"><span data-stu-id="f927e-130">displayName</span></span>|<span data-ttu-id="f927e-131">字符串</span><span class="sxs-lookup"><span data-stu-id="f927e-131">String</span></span>|<span data-ttu-id="f927e-132">协议的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f927e-132">Display name of the agreement.</span></span> <span data-ttu-id="f927e-133">The 显示名称 is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span><span class="sxs-lookup"><span data-stu-id="f927e-133">The display name is used for internal tracking of the agreement but is not shown to end users who view the agreement.</span></span>|
|<span data-ttu-id="f927e-134">id</span><span class="sxs-lookup"><span data-stu-id="f927e-134">id</span></span>|<span data-ttu-id="f927e-135">字符串</span><span class="sxs-lookup"><span data-stu-id="f927e-135">String</span></span>| <span data-ttu-id="f927e-136">协议的标识符。</span><span class="sxs-lookup"><span data-stu-id="f927e-136">The identifier of the agreement.</span></span> <span data-ttu-id="f927e-137">只读。</span><span class="sxs-lookup"><span data-stu-id="f927e-137">Read-only.</span></span>|
|<span data-ttu-id="f927e-138">isPerDeviceAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="f927e-138">isPerDeviceAcceptanceRequired</span></span>|<span data-ttu-id="f927e-139">布尔值</span><span class="sxs-lookup"><span data-stu-id="f927e-139">Boolean</span></span>|<span data-ttu-id="f927e-140">指示最终用户是否需要在从其访问它的每个设备上接受此协议。</span><span class="sxs-lookup"><span data-stu-id="f927e-140">Indicates whether end users are required to accept this agreement on every device that they access it from.</span></span> <span data-ttu-id="f927e-141">如果最终用户尚未在 Azure AD 中注册其设备，则要求他们这样做。</span><span class="sxs-lookup"><span data-stu-id="f927e-141">The end user is required to register their device in Azure AD, if they haven't already done so.</span></span>|
|<span data-ttu-id="f927e-142">isViewingBeforeAcceptanceRequired</span><span class="sxs-lookup"><span data-stu-id="f927e-142">isViewingBeforeAcceptanceRequired</span></span>|<span data-ttu-id="f927e-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="f927e-143">Boolean</span></span>|<span data-ttu-id="f927e-144">指示用户是否必须扩展协议才能接受。</span><span class="sxs-lookup"><span data-stu-id="f927e-144">Indicates whether the user has to expand the agreement before accepting.</span></span>|
|<span data-ttu-id="f927e-145">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="f927e-145">termsExpiration</span></span>|[<span data-ttu-id="f927e-146">termsExpiration</span><span class="sxs-lookup"><span data-stu-id="f927e-146">termsExpiration</span></span>](termsexpiration.md)| <span data-ttu-id="f927e-147">所有用户的过期日程安排和协议频率。</span><span class="sxs-lookup"><span data-stu-id="f927e-147">Expiration schedule and frequency of agreement for all users.</span></span> |
|<span data-ttu-id="f927e-148">userReacceptRequiredFrequency</span><span class="sxs-lookup"><span data-stu-id="f927e-148">userReacceptRequiredFrequency</span></span>|<span data-ttu-id="f927e-149">持续时间</span><span class="sxs-lookup"><span data-stu-id="f927e-149">Duration</span></span>|<span data-ttu-id="f927e-150">用户必须重新接受使用条款的持续时间。</span><span class="sxs-lookup"><span data-stu-id="f927e-150">The duration after which the user must re-accept the terms of use.</span></span> <span data-ttu-id="f927e-151">该值以 ISO 8601 格式表示持续时间。</span><span class="sxs-lookup"><span data-stu-id="f927e-151">The value is represented in ISO 8601 format for durations.</span></span>|


## <a name="relationships"></a><span data-ttu-id="f927e-152">关系</span><span class="sxs-lookup"><span data-stu-id="f927e-152">Relationships</span></span>
| <span data-ttu-id="f927e-153">关系</span><span class="sxs-lookup"><span data-stu-id="f927e-153">Relationship</span></span> | <span data-ttu-id="f927e-154">类型</span><span class="sxs-lookup"><span data-stu-id="f927e-154">Type</span></span>        | <span data-ttu-id="f927e-155">说明</span><span class="sxs-lookup"><span data-stu-id="f927e-155">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f927e-156">接受</span><span class="sxs-lookup"><span data-stu-id="f927e-156">acceptances</span></span>|<span data-ttu-id="f927e-157">[agreementAcceptance](agreementacceptance.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f927e-157">[agreementAcceptance](agreementacceptance.md) collection</span></span>|<span data-ttu-id="f927e-158">只读。</span><span class="sxs-lookup"><span data-stu-id="f927e-158">Read-only.</span></span> <span data-ttu-id="f927e-159">有关接受本协议的信息。</span><span class="sxs-lookup"><span data-stu-id="f927e-159">Information about acceptances of this agreement.</span></span>|
|<span data-ttu-id="f927e-160">files</span><span class="sxs-lookup"><span data-stu-id="f927e-160">files</span></span>|<span data-ttu-id="f927e-161">[agreementFileLocalization](agreementfilelocalization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f927e-161">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>| <span data-ttu-id="f927e-162">链接到本协议的 PDF。</span><span class="sxs-lookup"><span data-stu-id="f927e-162">PDFs linked to this agreement.</span></span> <span data-ttu-id="f927e-163">此属性正在被弃用。</span><span class="sxs-lookup"><span data-stu-id="f927e-163">This property is in the process of being deprecated.</span></span> <span data-ttu-id="f927e-164">请  **改为使用 file** 属性。</span><span class="sxs-lookup"><span data-stu-id="f927e-164">Use the  **file** property instead.</span></span>|
|<span data-ttu-id="f927e-165">file</span><span class="sxs-lookup"><span data-stu-id="f927e-165">file</span></span>|[<span data-ttu-id="f927e-166">agreementFile</span><span class="sxs-lookup"><span data-stu-id="f927e-166">agreementFile</span></span>](agreementfile.md) | <span data-ttu-id="f927e-167">链接到本协议的默认 PDF。</span><span class="sxs-lookup"><span data-stu-id="f927e-167">Default PDF linked to this agreement.</span></span>|
|<span data-ttu-id="f927e-168">本地化</span><span class="sxs-lookup"><span data-stu-id="f927e-168">localizations</span></span>|<span data-ttu-id="f927e-169">[agreementFileLocalization](agreementfilelocalization.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f927e-169">[agreementFileLocalization](agreementfilelocalization.md) collection</span></span>|<span data-ttu-id="f927e-170">附加到该协议的协议文件的本地化版本。</span><span class="sxs-lookup"><span data-stu-id="f927e-170">The localized versions of the agreement files attached to the agreement.</span></span>|
|<span data-ttu-id="f927e-171">版本</span><span class="sxs-lookup"><span data-stu-id="f927e-171">versions</span></span>|<span data-ttu-id="f927e-172">[agreementFileVersion](agreementfileversion.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f927e-172">[agreementFileVersion](agreementfileversion.md) collection</span></span>|<span data-ttu-id="f927e-173">本地化协议文件的版本历史记录。</span><span class="sxs-lookup"><span data-stu-id="f927e-173">The version history for the localized agreement file.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="f927e-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f927e-174">JSON representation</span></span>

<span data-ttu-id="f927e-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f927e-175">The following is a JSON representation of the resource.</span></span>

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


