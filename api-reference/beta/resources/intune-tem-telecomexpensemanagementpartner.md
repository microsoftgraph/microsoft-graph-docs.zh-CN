---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e1d148366a9ff67b643bad37e6aef5ed67653d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401850"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="4171f-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="4171f-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="4171f-105">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="4171f-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4171f-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4171f-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4171f-107">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4171f-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4171f-108">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="4171f-108">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="4171f-109">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="4171f-109">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>

## <a name="methods"></a><span data-ttu-id="4171f-110">方法</span><span class="sxs-lookup"><span data-stu-id="4171f-110">Methods</span></span>
|<span data-ttu-id="4171f-111">方法</span><span class="sxs-lookup"><span data-stu-id="4171f-111">Method</span></span>|<span data-ttu-id="4171f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="4171f-112">Return Type</span></span>|<span data-ttu-id="4171f-113">说明</span><span class="sxs-lookup"><span data-stu-id="4171f-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4171f-114">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="4171f-114">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="4171f-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4171f-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="4171f-116">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4171f-116">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="4171f-117">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-117">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="4171f-118">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-118">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="4171f-119">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4171f-119">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="4171f-120">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-120">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="4171f-121">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-121">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="4171f-122">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4171f-122">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="4171f-123">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-123">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="4171f-124">无</span><span class="sxs-lookup"><span data-stu-id="4171f-124">None</span></span>|<span data-ttu-id="4171f-125">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="4171f-125">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="4171f-126">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-126">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="4171f-127">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="4171f-127">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="4171f-128">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4171f-128">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4171f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4171f-129">Properties</span></span>
|<span data-ttu-id="4171f-130">属性</span><span class="sxs-lookup"><span data-stu-id="4171f-130">Property</span></span>|<span data-ttu-id="4171f-131">类型</span><span class="sxs-lookup"><span data-stu-id="4171f-131">Type</span></span>|<span data-ttu-id="4171f-132">说明</span><span class="sxs-lookup"><span data-stu-id="4171f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4171f-133">id</span><span class="sxs-lookup"><span data-stu-id="4171f-133">id</span></span>|<span data-ttu-id="4171f-134">String</span><span class="sxs-lookup"><span data-stu-id="4171f-134">String</span></span>|<span data-ttu-id="4171f-135">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4171f-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="4171f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4171f-136">displayName</span></span>|<span data-ttu-id="4171f-137">String</span><span class="sxs-lookup"><span data-stu-id="4171f-137">String</span></span>|<span data-ttu-id="4171f-138">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4171f-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="4171f-139">url</span><span class="sxs-lookup"><span data-stu-id="4171f-139">url</span></span>|<span data-ttu-id="4171f-140">String</span><span class="sxs-lookup"><span data-stu-id="4171f-140">String</span></span>|<span data-ttu-id="4171f-141">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="4171f-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="4171f-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="4171f-142">appAuthorized</span></span>|<span data-ttu-id="4171f-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-143">Boolean</span></span>|<span data-ttu-id="4171f-144">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="4171f-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="4171f-145">enabled</span><span class="sxs-lookup"><span data-stu-id="4171f-145">enabled</span></span>|<span data-ttu-id="4171f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="4171f-146">Boolean</span></span>|<span data-ttu-id="4171f-147">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="4171f-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="4171f-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="4171f-148">lastConnectionDateTime</span></span>|<span data-ttu-id="4171f-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4171f-149">DateTimeOffset</span></span>|<span data-ttu-id="4171f-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="4171f-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4171f-151">关系</span><span class="sxs-lookup"><span data-stu-id="4171f-151">Relationships</span></span>
<span data-ttu-id="4171f-152">无</span><span class="sxs-lookup"><span data-stu-id="4171f-152">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4171f-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4171f-153">JSON Representation</span></span>
<span data-ttu-id="4171f-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4171f-154">Here is a JSON representation of the resource.</span></span>
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




