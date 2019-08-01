---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c73674c0854c2367fb988dde6f21eb0db6a64d59
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036797"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="8ff2b-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ff2b-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="8ff2b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8ff2b-106">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-106">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="8ff2b-107">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-107">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="8ff2b-108">方法</span><span class="sxs-lookup"><span data-stu-id="8ff2b-108">Methods</span></span>
|<span data-ttu-id="8ff2b-109">方法</span><span class="sxs-lookup"><span data-stu-id="8ff2b-109">Method</span></span>|<span data-ttu-id="8ff2b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ff2b-110">Return Type</span></span>|<span data-ttu-id="8ff2b-111">说明</span><span class="sxs-lookup"><span data-stu-id="8ff2b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8ff2b-112">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="8ff2b-112">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="8ff2b-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ff2b-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="8ff2b-114">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-114">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="8ff2b-115">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-115">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="8ff2b-116">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-116">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8ff2b-117">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-117">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="8ff2b-118">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-118">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="8ff2b-119">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-119">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8ff2b-120">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-120">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="8ff2b-121">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-121">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="8ff2b-122">无</span><span class="sxs-lookup"><span data-stu-id="8ff2b-122">None</span></span>|<span data-ttu-id="8ff2b-123">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-123">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="8ff2b-124">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-124">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="8ff2b-125">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="8ff2b-125">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="8ff2b-126">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-126">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8ff2b-127">属性</span><span class="sxs-lookup"><span data-stu-id="8ff2b-127">Properties</span></span>
|<span data-ttu-id="8ff2b-128">属性</span><span class="sxs-lookup"><span data-stu-id="8ff2b-128">Property</span></span>|<span data-ttu-id="8ff2b-129">类型</span><span class="sxs-lookup"><span data-stu-id="8ff2b-129">Type</span></span>|<span data-ttu-id="8ff2b-130">说明</span><span class="sxs-lookup"><span data-stu-id="8ff2b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8ff2b-131">id</span><span class="sxs-lookup"><span data-stu-id="8ff2b-131">id</span></span>|<span data-ttu-id="8ff2b-132">String</span><span class="sxs-lookup"><span data-stu-id="8ff2b-132">String</span></span>|<span data-ttu-id="8ff2b-133">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="8ff2b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="8ff2b-134">displayName</span></span>|<span data-ttu-id="8ff2b-135">字符串</span><span class="sxs-lookup"><span data-stu-id="8ff2b-135">String</span></span>|<span data-ttu-id="8ff2b-136">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="8ff2b-137">url</span><span class="sxs-lookup"><span data-stu-id="8ff2b-137">url</span></span>|<span data-ttu-id="8ff2b-138">String</span><span class="sxs-lookup"><span data-stu-id="8ff2b-138">String</span></span>|<span data-ttu-id="8ff2b-139">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="8ff2b-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="8ff2b-140">appAuthorized</span></span>|<span data-ttu-id="8ff2b-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ff2b-141">Boolean</span></span>|<span data-ttu-id="8ff2b-142">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="8ff2b-143">enabled</span><span class="sxs-lookup"><span data-stu-id="8ff2b-143">enabled</span></span>|<span data-ttu-id="8ff2b-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="8ff2b-144">Boolean</span></span>|<span data-ttu-id="8ff2b-145">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="8ff2b-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8ff2b-146">lastConnectionDateTime</span></span>|<span data-ttu-id="8ff2b-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ff2b-147">DateTimeOffset</span></span>|<span data-ttu-id="8ff2b-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8ff2b-149">关系</span><span class="sxs-lookup"><span data-stu-id="8ff2b-149">Relationships</span></span>
<span data-ttu-id="8ff2b-150">无</span><span class="sxs-lookup"><span data-stu-id="8ff2b-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8ff2b-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ff2b-151">JSON Representation</span></span>
<span data-ttu-id="8ff2b-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ff2b-152">Here is a JSON representation of the resource.</span></span>
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



