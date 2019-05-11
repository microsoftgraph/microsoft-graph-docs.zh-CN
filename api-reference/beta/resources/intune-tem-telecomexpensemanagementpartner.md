---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7479619bf7493ca2f043d7423d994f9fb0b6f905
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939824"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="28b59-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="28b59-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="28b59-105">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="28b59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="28b59-106">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="28b59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="28b59-107">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="28b59-107">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="28b59-108">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="28b59-108">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="28b59-109">方法</span><span class="sxs-lookup"><span data-stu-id="28b59-109">Methods</span></span>
|<span data-ttu-id="28b59-110">方法</span><span class="sxs-lookup"><span data-stu-id="28b59-110">Method</span></span>|<span data-ttu-id="28b59-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="28b59-111">Return Type</span></span>|<span data-ttu-id="28b59-112">说明</span><span class="sxs-lookup"><span data-stu-id="28b59-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="28b59-113">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="28b59-113">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="28b59-114">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28b59-114">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="28b59-115">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="28b59-115">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="28b59-116">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-116">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="28b59-117">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-117">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="28b59-118">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="28b59-118">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="28b59-119">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-119">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="28b59-120">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-120">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="28b59-121">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28b59-121">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="28b59-122">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-122">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="28b59-123">无</span><span class="sxs-lookup"><span data-stu-id="28b59-123">None</span></span>|<span data-ttu-id="28b59-124">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="28b59-124">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="28b59-125">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-125">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="28b59-126">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="28b59-126">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="28b59-127">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="28b59-127">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="28b59-128">属性</span><span class="sxs-lookup"><span data-stu-id="28b59-128">Properties</span></span>
|<span data-ttu-id="28b59-129">属性</span><span class="sxs-lookup"><span data-stu-id="28b59-129">Property</span></span>|<span data-ttu-id="28b59-130">类型</span><span class="sxs-lookup"><span data-stu-id="28b59-130">Type</span></span>|<span data-ttu-id="28b59-131">说明</span><span class="sxs-lookup"><span data-stu-id="28b59-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="28b59-132">id</span><span class="sxs-lookup"><span data-stu-id="28b59-132">id</span></span>|<span data-ttu-id="28b59-133">String</span><span class="sxs-lookup"><span data-stu-id="28b59-133">String</span></span>|<span data-ttu-id="28b59-134">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="28b59-134">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="28b59-135">displayName</span><span class="sxs-lookup"><span data-stu-id="28b59-135">displayName</span></span>|<span data-ttu-id="28b59-136">字符串</span><span class="sxs-lookup"><span data-stu-id="28b59-136">String</span></span>|<span data-ttu-id="28b59-137">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="28b59-137">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="28b59-138">url</span><span class="sxs-lookup"><span data-stu-id="28b59-138">url</span></span>|<span data-ttu-id="28b59-139">String</span><span class="sxs-lookup"><span data-stu-id="28b59-139">String</span></span>|<span data-ttu-id="28b59-140">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="28b59-140">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="28b59-141">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="28b59-141">appAuthorized</span></span>|<span data-ttu-id="28b59-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="28b59-142">Boolean</span></span>|<span data-ttu-id="28b59-143">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="28b59-143">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="28b59-144">enabled</span><span class="sxs-lookup"><span data-stu-id="28b59-144">enabled</span></span>|<span data-ttu-id="28b59-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="28b59-145">Boolean</span></span>|<span data-ttu-id="28b59-146">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="28b59-146">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="28b59-147">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="28b59-147">lastConnectionDateTime</span></span>|<span data-ttu-id="28b59-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="28b59-148">DateTimeOffset</span></span>|<span data-ttu-id="28b59-149">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="28b59-149">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28b59-150">关系</span><span class="sxs-lookup"><span data-stu-id="28b59-150">Relationships</span></span>
<span data-ttu-id="28b59-151">无</span><span class="sxs-lookup"><span data-stu-id="28b59-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="28b59-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28b59-152">JSON Representation</span></span>
<span data-ttu-id="28b59-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28b59-153">Here is a JSON representation of the resource.</span></span>
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




