---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c941ce38e57251e22df473b279d151a35f5259eb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089334"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="53d3d-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="53d3d-104">telecomExpenseManagementPartner resource type</span></span>

<span data-ttu-id="53d3d-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53d3d-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53d3d-106">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="53d3d-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53d3d-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53d3d-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53d3d-108">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="53d3d-108">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="53d3d-109">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="53d3d-109">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="53d3d-110">方法</span><span class="sxs-lookup"><span data-stu-id="53d3d-110">Methods</span></span>
|<span data-ttu-id="53d3d-111">方法</span><span class="sxs-lookup"><span data-stu-id="53d3d-111">Method</span></span>|<span data-ttu-id="53d3d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="53d3d-112">Return Type</span></span>|<span data-ttu-id="53d3d-113">说明</span><span class="sxs-lookup"><span data-stu-id="53d3d-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53d3d-114">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="53d3d-114">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="53d3d-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="53d3d-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="53d3d-116">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53d3d-116">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="53d3d-117">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-117">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="53d3d-118">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-118">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="53d3d-119">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="53d3d-119">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="53d3d-120">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-120">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="53d3d-121">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-121">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="53d3d-122">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53d3d-122">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="53d3d-123">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-123">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="53d3d-124">无</span><span class="sxs-lookup"><span data-stu-id="53d3d-124">None</span></span>|<span data-ttu-id="53d3d-125">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="53d3d-125">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="53d3d-126">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-126">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="53d3d-127">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="53d3d-127">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="53d3d-128">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53d3d-128">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="53d3d-129">属性</span><span class="sxs-lookup"><span data-stu-id="53d3d-129">Properties</span></span>
|<span data-ttu-id="53d3d-130">属性</span><span class="sxs-lookup"><span data-stu-id="53d3d-130">Property</span></span>|<span data-ttu-id="53d3d-131">类型</span><span class="sxs-lookup"><span data-stu-id="53d3d-131">Type</span></span>|<span data-ttu-id="53d3d-132">说明</span><span class="sxs-lookup"><span data-stu-id="53d3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53d3d-133">id</span><span class="sxs-lookup"><span data-stu-id="53d3d-133">id</span></span>|<span data-ttu-id="53d3d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="53d3d-134">String</span></span>|<span data-ttu-id="53d3d-135">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="53d3d-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="53d3d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="53d3d-136">displayName</span></span>|<span data-ttu-id="53d3d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="53d3d-137">String</span></span>|<span data-ttu-id="53d3d-138">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="53d3d-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="53d3d-139">url</span><span class="sxs-lookup"><span data-stu-id="53d3d-139">url</span></span>|<span data-ttu-id="53d3d-140">String</span><span class="sxs-lookup"><span data-stu-id="53d3d-140">String</span></span>|<span data-ttu-id="53d3d-141">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="53d3d-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="53d3d-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="53d3d-142">appAuthorized</span></span>|<span data-ttu-id="53d3d-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="53d3d-143">Boolean</span></span>|<span data-ttu-id="53d3d-144">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="53d3d-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="53d3d-145">enabled</span><span class="sxs-lookup"><span data-stu-id="53d3d-145">enabled</span></span>|<span data-ttu-id="53d3d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="53d3d-146">Boolean</span></span>|<span data-ttu-id="53d3d-147">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="53d3d-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="53d3d-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="53d3d-148">lastConnectionDateTime</span></span>|<span data-ttu-id="53d3d-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53d3d-149">DateTimeOffset</span></span>|<span data-ttu-id="53d3d-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="53d3d-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="53d3d-151">关系</span><span class="sxs-lookup"><span data-stu-id="53d3d-151">Relationships</span></span>
<span data-ttu-id="53d3d-152">无</span><span class="sxs-lookup"><span data-stu-id="53d3d-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53d3d-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53d3d-153">JSON Representation</span></span>
<span data-ttu-id="53d3d-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53d3d-154">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.telecomExpenseManagementPartner"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "String (identifier)",
  "displayName": "String",
  "url": "String",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "String (timestamp)"
}
```






