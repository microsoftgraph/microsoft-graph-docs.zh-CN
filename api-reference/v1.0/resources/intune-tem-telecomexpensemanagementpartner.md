---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: c515b21f5727bcb60588a6722cc3fd6b02719e36
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981796"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="38aba-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="38aba-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="38aba-105">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="38aba-105">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="38aba-106">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="38aba-106">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="38aba-107">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="38aba-107">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>
## <a name="methods"></a><span data-ttu-id="38aba-108">方法</span><span class="sxs-lookup"><span data-stu-id="38aba-108">Methods</span></span>
|<span data-ttu-id="38aba-109">方法</span><span class="sxs-lookup"><span data-stu-id="38aba-109">Method</span></span>|<span data-ttu-id="38aba-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="38aba-110">Return Type</span></span>|<span data-ttu-id="38aba-111">说明</span><span class="sxs-lookup"><span data-stu-id="38aba-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="38aba-112">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="38aba-112">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="38aba-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="38aba-113">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="38aba-114">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38aba-114">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="38aba-115">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-115">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="38aba-116">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-116">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="38aba-117">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="38aba-117">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="38aba-118">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-118">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="38aba-119">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-119">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="38aba-120">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="38aba-120">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="38aba-121">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-121">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="38aba-122">无</span><span class="sxs-lookup"><span data-stu-id="38aba-122">None</span></span>|<span data-ttu-id="38aba-123">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="38aba-123">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="38aba-124">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-124">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="38aba-125">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="38aba-125">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="38aba-126">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="38aba-126">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="38aba-127">属性</span><span class="sxs-lookup"><span data-stu-id="38aba-127">Properties</span></span>
|<span data-ttu-id="38aba-128">属性</span><span class="sxs-lookup"><span data-stu-id="38aba-128">Property</span></span>|<span data-ttu-id="38aba-129">类型</span><span class="sxs-lookup"><span data-stu-id="38aba-129">Type</span></span>|<span data-ttu-id="38aba-130">说明</span><span class="sxs-lookup"><span data-stu-id="38aba-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38aba-131">id</span><span class="sxs-lookup"><span data-stu-id="38aba-131">id</span></span>|<span data-ttu-id="38aba-132">String</span><span class="sxs-lookup"><span data-stu-id="38aba-132">String</span></span>|<span data-ttu-id="38aba-133">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="38aba-133">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="38aba-134">displayName</span><span class="sxs-lookup"><span data-stu-id="38aba-134">displayName</span></span>|<span data-ttu-id="38aba-135">String</span><span class="sxs-lookup"><span data-stu-id="38aba-135">String</span></span>|<span data-ttu-id="38aba-136">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="38aba-136">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="38aba-137">url</span><span class="sxs-lookup"><span data-stu-id="38aba-137">url</span></span>|<span data-ttu-id="38aba-138">String</span><span class="sxs-lookup"><span data-stu-id="38aba-138">String</span></span>|<span data-ttu-id="38aba-139">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="38aba-139">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="38aba-140">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="38aba-140">appAuthorized</span></span>|<span data-ttu-id="38aba-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="38aba-141">Boolean</span></span>|<span data-ttu-id="38aba-142">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="38aba-142">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="38aba-143">enabled</span><span class="sxs-lookup"><span data-stu-id="38aba-143">enabled</span></span>|<span data-ttu-id="38aba-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="38aba-144">Boolean</span></span>|<span data-ttu-id="38aba-145">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="38aba-145">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="38aba-146">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="38aba-146">lastConnectionDateTime</span></span>|<span data-ttu-id="38aba-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38aba-147">DateTimeOffset</span></span>|<span data-ttu-id="38aba-148">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="38aba-148">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="38aba-149">关系</span><span class="sxs-lookup"><span data-stu-id="38aba-149">Relationships</span></span>
<span data-ttu-id="38aba-150">无</span><span class="sxs-lookup"><span data-stu-id="38aba-150">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="38aba-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="38aba-151">JSON Representation</span></span>
<span data-ttu-id="38aba-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38aba-152">Here is a JSON representation of the resource.</span></span>
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



