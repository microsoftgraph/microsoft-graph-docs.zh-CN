---
title: legalHold 资源类型
description: legalHold 资源类型
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 4fa13783de13c216d8ec89aca67218e3eec56bfc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446622"
---
# <a name="legalhold-resource-type"></a><span data-ttu-id="03d15-103">legalHold 资源类型</span><span class="sxs-lookup"><span data-stu-id="03d15-103">legalHold resource type</span></span>

<span data-ttu-id="03d15-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="03d15-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03d15-105">表示法定保留。</span><span class="sxs-lookup"><span data-stu-id="03d15-105">Represents a legal hold.</span></span> <span data-ttu-id="03d15-106">合法保留与电子数据展示案例关联。</span><span class="sxs-lookup"><span data-stu-id="03d15-106">Legal holds are holds that are tied to an eDiscovery case.</span></span> <span data-ttu-id="03d15-107">不得将合法保留与保留保留混淆，保留保留用于控制 Microsoft 365 内容的保留策略。</span><span class="sxs-lookup"><span data-stu-id="03d15-107">Legal holds should not be confused with retention holds, which are used to control retention policies for Microsoft 365 content.</span></span> <span data-ttu-id="03d15-108">电子数据展示法律保留用于无限期保留内容，以用于需要防止删除内容的诉讼、内部调查和其他法律操作。</span><span class="sxs-lookup"><span data-stu-id="03d15-108">eDiscovery legal holds are for holding content indefinitely for litigation, internal investigations, and other legal actions where content needs to be protected against deletion.</span></span> <span data-ttu-id="03d15-109">有关详细信息，请参阅["管理高级电子数据展示中的保留](/microsoft-365/compliance/managing-holds)"</span><span class="sxs-lookup"><span data-stu-id="03d15-109">For more information, see [Manage holds in Advanced eDiscovery](/microsoft-365/compliance/managing-holds)</span></span>

<span data-ttu-id="03d15-110">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="03d15-110">Inherits from [entity](../resources/entity.md).</span></span>

## <a name="methods"></a><span data-ttu-id="03d15-111">Methods</span><span class="sxs-lookup"><span data-stu-id="03d15-111">Methods</span></span>

|<span data-ttu-id="03d15-112">方法</span><span class="sxs-lookup"><span data-stu-id="03d15-112">Method</span></span>|<span data-ttu-id="03d15-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="03d15-113">Return type</span></span>|<span data-ttu-id="03d15-114">说明</span><span class="sxs-lookup"><span data-stu-id="03d15-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03d15-115">列出 legalHolds</span><span class="sxs-lookup"><span data-stu-id="03d15-115">List legalHolds</span></span>](../api/ediscovery-case-list-legalholds.md)|<span data-ttu-id="03d15-116">[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03d15-116">[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) collection</span></span>|<span data-ttu-id="03d15-117">获取  **legalHold 对象及其** 属性的列表。</span><span class="sxs-lookup"><span data-stu-id="03d15-117">Get a list of the  **legalHold** objects and their properties.</span></span>|
|[<span data-ttu-id="03d15-118">创建 legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-118">Create legalHold</span></span>](../api/ediscovery-case-post-legalholds.md)|[<span data-ttu-id="03d15-119">microsoft.graph.ediscovery.legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-119">microsoft.graph.ediscovery.legalHold</span></span>](../resources/ediscovery-legalhold.md)|<span data-ttu-id="03d15-120">创建新的 **legalHold** 对象。</span><span class="sxs-lookup"><span data-stu-id="03d15-120">Create a new **legalHold** object.</span></span>|
|[<span data-ttu-id="03d15-121">获取 legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-121">Get legalHold</span></span>](../api/ediscovery-legalhold-get.md)|[<span data-ttu-id="03d15-122">microsoft.graph.ediscovery.legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-122">microsoft.graph.ediscovery.legalHold</span></span>](../resources/ediscovery-legalhold.md)|<span data-ttu-id="03d15-123">读取 **legalHold 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="03d15-123">Read the properties and relationships of a **legalHold** object.</span></span>|
|[<span data-ttu-id="03d15-124">更新 legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-124">Update legalHold</span></span>](../api/ediscovery-legalhold-update.md)|[<span data-ttu-id="03d15-125">microsoft.graph.ediscovery.legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-125">microsoft.graph.ediscovery.legalHold</span></span>](../resources/ediscovery-legalhold.md)|<span data-ttu-id="03d15-126">更新 **legalHold 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="03d15-126">Update the properties of a **legalHold** object.</span></span>|
|[<span data-ttu-id="03d15-127">删除 legalHold</span><span class="sxs-lookup"><span data-stu-id="03d15-127">Delete legalHold</span></span>](../api/ediscovery-legalhold-delete.md)|<span data-ttu-id="03d15-128">无</span><span class="sxs-lookup"><span data-stu-id="03d15-128">None</span></span>|<span data-ttu-id="03d15-129">删除 **legalHold** 对象。</span><span class="sxs-lookup"><span data-stu-id="03d15-129">Delete a **legalHold** object.</span></span>|
|[<span data-ttu-id="03d15-130">列出 siteSources</span><span class="sxs-lookup"><span data-stu-id="03d15-130">List siteSources</span></span>](../api/ediscovery-legalhold-list-sitesources.md)|<span data-ttu-id="03d15-131">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03d15-131">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="03d15-132">获取与合法保留相关联的 [siteSource](../resources/ediscovery-sitesource.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="03d15-132">Get the list of [siteSource](../resources/ediscovery-sitesource.md) objecs associated with a legal hold.</span></span>|
|[<span data-ttu-id="03d15-133">创建 siteSource</span><span class="sxs-lookup"><span data-stu-id="03d15-133">Create siteSource</span></span>](../api/ediscovery-legalhold-post-sitesources.md)|[<span data-ttu-id="03d15-134">microsoft.graph.ediscovery.siteSource</span><span class="sxs-lookup"><span data-stu-id="03d15-134">microsoft.graph.ediscovery.siteSource</span></span>](../resources/ediscovery-sitesource.md)|<span data-ttu-id="03d15-135">创建新的 siteSource 对象。</span><span class="sxs-lookup"><span data-stu-id="03d15-135">Create a new siteSource object.</span></span>|
|[<span data-ttu-id="03d15-136">列出 userSources</span><span class="sxs-lookup"><span data-stu-id="03d15-136">List userSources</span></span>](../api/ediscovery-legalhold-list-usersources.md)|<span data-ttu-id="03d15-137">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03d15-137">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>|<span data-ttu-id="03d15-138">获取与合法保留相关联的 [userSource](../resources/ediscovery-usersource.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="03d15-138">Get the list of [userSource](../resources/ediscovery-usersource.md) objects associated with a legal hold.</span></span>|
|[<span data-ttu-id="03d15-139">创建 userSource</span><span class="sxs-lookup"><span data-stu-id="03d15-139">Create userSource</span></span>](../api/ediscovery-legalhold-post-usersources.md)|[<span data-ttu-id="03d15-140">microsoft.graph.ediscovery.userSource</span><span class="sxs-lookup"><span data-stu-id="03d15-140">microsoft.graph.ediscovery.userSource</span></span>](../resources/ediscovery-usersource.md)|<span data-ttu-id="03d15-141">创建新的 **userSource** 对象。</span><span class="sxs-lookup"><span data-stu-id="03d15-141">Create a new **userSource** object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03d15-142">属性</span><span class="sxs-lookup"><span data-stu-id="03d15-142">Properties</span></span>

|<span data-ttu-id="03d15-143">属性</span><span class="sxs-lookup"><span data-stu-id="03d15-143">Property</span></span>|<span data-ttu-id="03d15-144">类型</span><span class="sxs-lookup"><span data-stu-id="03d15-144">Type</span></span>|<span data-ttu-id="03d15-145">说明</span><span class="sxs-lookup"><span data-stu-id="03d15-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d15-146">contentQuery</span><span class="sxs-lookup"><span data-stu-id="03d15-146">contentQuery</span></span>|<span data-ttu-id="03d15-147">String</span><span class="sxs-lookup"><span data-stu-id="03d15-147">String</span></span>|<span data-ttu-id="03d15-148">指定要位于指定位置的内容的 KQL 查询。</span><span class="sxs-lookup"><span data-stu-id="03d15-148">KQL query that specifies content to be held in the specified locations.</span></span> <span data-ttu-id="03d15-149">若要了解更多信息，请参阅内容搜索和电子数据展示的关键字 [查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。</span><span class="sxs-lookup"><span data-stu-id="03d15-149">To learn more, see [Keyword queries and search conditions for Content Search and eDiscovery](/microsoft-365/compliance/keyword-queries-and-search-conditions).</span></span>  <span data-ttu-id="03d15-150">若要保留指定位置中所有内容，请保留 **contentQuery** 为空。</span><span class="sxs-lookup"><span data-stu-id="03d15-150">To hold all content in the specified locations, leave **contentQuery** blank.</span></span> |
|<span data-ttu-id="03d15-151">createdBy</span><span class="sxs-lookup"><span data-stu-id="03d15-151">createdBy</span></span>|[<span data-ttu-id="03d15-152">identitySet</span><span class="sxs-lookup"><span data-stu-id="03d15-152">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="03d15-153">创建合法保留的用户。</span><span class="sxs-lookup"><span data-stu-id="03d15-153">The user who created the legal hold.</span></span> |
|<span data-ttu-id="03d15-154">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="03d15-154">createdDateTime</span></span>|<span data-ttu-id="03d15-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03d15-155">DateTimeOffset</span></span>|<span data-ttu-id="03d15-156">创建合法保留的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03d15-156">The date and time the legal hold was created.</span></span> |
|<span data-ttu-id="03d15-157">说明</span><span class="sxs-lookup"><span data-stu-id="03d15-157">description</span></span>|<span data-ttu-id="03d15-158">String</span><span class="sxs-lookup"><span data-stu-id="03d15-158">String</span></span>| <span data-ttu-id="03d15-159">法定保留说明。</span><span class="sxs-lookup"><span data-stu-id="03d15-159">The legal hold description.</span></span> |
|<span data-ttu-id="03d15-160">displayName</span><span class="sxs-lookup"><span data-stu-id="03d15-160">displayName</span></span>|<span data-ttu-id="03d15-161">String</span><span class="sxs-lookup"><span data-stu-id="03d15-161">String</span></span>| <span data-ttu-id="03d15-162">法定显示名称的一部分。</span><span class="sxs-lookup"><span data-stu-id="03d15-162">The display name of the legal hold.</span></span> |
|<span data-ttu-id="03d15-163">错误</span><span class="sxs-lookup"><span data-stu-id="03d15-163">errors</span></span>|<span data-ttu-id="03d15-164">字符串集合</span><span class="sxs-lookup"><span data-stu-id="03d15-164">String collection</span></span>|<span data-ttu-id="03d15-165">列出置于保留时发生的任何错误。</span><span class="sxs-lookup"><span data-stu-id="03d15-165">Lists any errors that happened while placing the hold.</span></span> |
|<span data-ttu-id="03d15-166">id</span><span class="sxs-lookup"><span data-stu-id="03d15-166">id</span></span>|<span data-ttu-id="03d15-167">String</span><span class="sxs-lookup"><span data-stu-id="03d15-167">String</span></span>|<span data-ttu-id="03d15-168">电子数据展示案例的 ID。</span><span class="sxs-lookup"><span data-stu-id="03d15-168">The ID for the eDiscovery case.</span></span> <span data-ttu-id="03d15-169">只读。</span><span class="sxs-lookup"><span data-stu-id="03d15-169">Read-only.</span></span> <span data-ttu-id="03d15-170">继承自 [实体](../resources/entity.md)。</span><span class="sxs-lookup"><span data-stu-id="03d15-170">Inherited from [entity](../resources/entity.md).</span></span> |
|<span data-ttu-id="03d15-171">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03d15-171">isEnabled</span></span>|<span data-ttu-id="03d15-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="03d15-172">Boolean</span></span>|<span data-ttu-id="03d15-173">指示是否启用保留并主动保留内容。</span><span class="sxs-lookup"><span data-stu-id="03d15-173">Indicates whether the hold is enabled and actively holding content.</span></span> |
|<span data-ttu-id="03d15-174">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="03d15-174">lastModifiedBy</span></span>|[<span data-ttu-id="03d15-175">identitySet</span><span class="sxs-lookup"><span data-stu-id="03d15-175">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="03d15-176">上次修改法定保留的用户。</span><span class="sxs-lookup"><span data-stu-id="03d15-176">the user who last modified the legal hold.</span></span>|
|<span data-ttu-id="03d15-177">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="03d15-177">lastModifiedDateTime</span></span>|<span data-ttu-id="03d15-178">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03d15-178">DateTimeOffset</span></span>|<span data-ttu-id="03d15-179">上次修改合法保留的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="03d15-179">The date and time the legal hold was last modified.</span></span> |
|<span data-ttu-id="03d15-180">status</span><span class="sxs-lookup"><span data-stu-id="03d15-180">status</span></span>|<span data-ttu-id="03d15-181">microsoft.graph.ediscovery.legalHoldStatus</span><span class="sxs-lookup"><span data-stu-id="03d15-181">microsoft.graph.ediscovery.legalHoldStatus</span></span>|<span data-ttu-id="03d15-182">合法保留的状态。</span><span class="sxs-lookup"><span data-stu-id="03d15-182">The status of the legal hold.</span></span> <span data-ttu-id="03d15-183">可取值为：`Pending`、`Error`、`Success`、`UnknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="03d15-183">Possible values are: `Pending`, `Error`, `Success`, `UnknownFutureValue`.</span></span>|

### <a name="legalholdstatus-values"></a><span data-ttu-id="03d15-184">legalHoldStatus 值</span><span class="sxs-lookup"><span data-stu-id="03d15-184">legalHoldStatus values</span></span>

|<span data-ttu-id="03d15-185">成员</span><span class="sxs-lookup"><span data-stu-id="03d15-185">Member</span></span>|<span data-ttu-id="03d15-186">说明</span><span class="sxs-lookup"><span data-stu-id="03d15-186">Description</span></span>|
|:---|-----------|
|<span data-ttu-id="03d15-187">Pending</span><span class="sxs-lookup"><span data-stu-id="03d15-187">Pending</span></span>| <span data-ttu-id="03d15-188">保留分发过程正在进行中。</span><span class="sxs-lookup"><span data-stu-id="03d15-188">The hold distribution process is in progress.</span></span> |
|<span data-ttu-id="03d15-189">错误</span><span class="sxs-lookup"><span data-stu-id="03d15-189">Error</span></span>| <span data-ttu-id="03d15-190">应用保留时出错。</span><span class="sxs-lookup"><span data-stu-id="03d15-190">There was an error when the hold was applied.</span></span> <span data-ttu-id="03d15-191">有关详细信息，请参阅 legalHold 对象的 errors 属性。</span><span class="sxs-lookup"><span data-stu-id="03d15-191">For details, see the errors property of the legalHold object.</span></span> |
|<span data-ttu-id="03d15-192">成功</span><span class="sxs-lookup"><span data-stu-id="03d15-192">Success</span></span>| <span data-ttu-id="03d15-193">已成功应用保留并保留指定内容。</span><span class="sxs-lookup"><span data-stu-id="03d15-193">The hold was successfully applied and is holding the specified content.</span></span> |

## <a name="relationships"></a><span data-ttu-id="03d15-194">关系</span><span class="sxs-lookup"><span data-stu-id="03d15-194">Relationships</span></span>

|<span data-ttu-id="03d15-195">关系</span><span class="sxs-lookup"><span data-stu-id="03d15-195">Relationship</span></span>|<span data-ttu-id="03d15-196">类型</span><span class="sxs-lookup"><span data-stu-id="03d15-196">Type</span></span>|<span data-ttu-id="03d15-197">说明</span><span class="sxs-lookup"><span data-stu-id="03d15-197">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03d15-198">siteSources</span><span class="sxs-lookup"><span data-stu-id="03d15-198">siteSources</span></span>|<span data-ttu-id="03d15-199">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03d15-199">[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) collection</span></span>|<span data-ttu-id="03d15-200">与法定保留相关联的 SharePoint 网站的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="03d15-200">Data source entity for SharePoint sites associated with the legal hold.</span></span> |
|<span data-ttu-id="03d15-201">userSources</span><span class="sxs-lookup"><span data-stu-id="03d15-201">userSources</span></span>|<span data-ttu-id="03d15-202">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03d15-202">[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) collection</span></span>| <span data-ttu-id="03d15-203">合法保留的数据源实体。</span><span class="sxs-lookup"><span data-stu-id="03d15-203">Data source entity for a the legal hold.</span></span> <span data-ttu-id="03d15-204">这是邮箱和 OneDrive for Business 网站的容器。</span><span class="sxs-lookup"><span data-stu-id="03d15-204">This is the container for a mailbox and OneDrive for Business site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="03d15-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03d15-205">JSON representation</span></span>

<span data-ttu-id="03d15-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03d15-206">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.legalHold",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "String (identifier)",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
