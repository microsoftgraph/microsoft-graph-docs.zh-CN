---
title: telecomExpenseManagementPartner 资源类型
description: telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。 组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。
ms.openlocfilehash: 1418f40b5de113e3d46a20e6bf2bb190709def89
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047190"
---
# <a name="telecomexpensemanagementpartner-resource-type"></a><span data-ttu-id="85263-104">telecomExpenseManagementPartner 资源类型</span><span class="sxs-lookup"><span data-stu-id="85263-104">telecomExpenseManagementPartner resource type</span></span>

> <span data-ttu-id="85263-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85263-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85263-106">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85263-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85263-107">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="85263-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85263-108">telecomExpenseManagementPartner 资源表示给定 TEM 服务的元数据和状态。</span><span class="sxs-lookup"><span data-stu-id="85263-108">telecomExpenseManagementPartner resources represent the metadata and status of a given TEM service.</span></span> <span data-ttu-id="85263-109">组织通过合作伙伴载入后，即可允许或禁止合作伙伴打开或关闭 TEM 功能。</span><span class="sxs-lookup"><span data-stu-id="85263-109">Once your organization has onboarded with a partner, the partner can be enabled or disabled to switch TEM functionality on or off.</span></span>
## <a name="methods"></a><span data-ttu-id="85263-110">方法</span><span class="sxs-lookup"><span data-stu-id="85263-110">Methods</span></span>
|<span data-ttu-id="85263-111">方法</span><span class="sxs-lookup"><span data-stu-id="85263-111">Method</span></span>|<span data-ttu-id="85263-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="85263-112">Return Type</span></span>|<span data-ttu-id="85263-113">说明</span><span class="sxs-lookup"><span data-stu-id="85263-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85263-114">List telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="85263-114">List telecomExpenseManagementPartners</span></span>](../api/intune-tem-telecomexpensemanagementpartner-list.md)|<span data-ttu-id="85263-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 集合</span><span class="sxs-lookup"><span data-stu-id="85263-115">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="85263-116">列出 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="85263-116">List properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) objects.</span></span>|
|[<span data-ttu-id="85263-117">Get telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-117">Get telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-get.md)|[<span data-ttu-id="85263-118">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-118">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="85263-119">读取 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="85263-119">Read properties and relationships of the [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="85263-120">Create telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-120">Create telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-create.md)|[<span data-ttu-id="85263-121">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-121">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="85263-122">创建新的 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="85263-122">Create a new [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|
|[<span data-ttu-id="85263-123">Delete telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-123">Delete telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-delete.md)|<span data-ttu-id="85263-124">无</span><span class="sxs-lookup"><span data-stu-id="85263-124">None</span></span>|<span data-ttu-id="85263-125">删除 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)。</span><span class="sxs-lookup"><span data-stu-id="85263-125">Deletes a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md).</span></span>|
|[<span data-ttu-id="85263-126">Update telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-126">Update telecomExpenseManagementPartner</span></span>](../api/intune-tem-telecomexpensemanagementpartner-update.md)|[<span data-ttu-id="85263-127">telecomExpenseManagementPartner</span><span class="sxs-lookup"><span data-stu-id="85263-127">telecomExpenseManagementPartner</span></span>](../resources/intune-tem-telecomexpensemanagementpartner.md)|<span data-ttu-id="85263-128">更新 [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="85263-128">Update the properties of a [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="85263-129">属性</span><span class="sxs-lookup"><span data-stu-id="85263-129">Properties</span></span>
|<span data-ttu-id="85263-130">属性</span><span class="sxs-lookup"><span data-stu-id="85263-130">Property</span></span>|<span data-ttu-id="85263-131">类型</span><span class="sxs-lookup"><span data-stu-id="85263-131">Type</span></span>|<span data-ttu-id="85263-132">说明</span><span class="sxs-lookup"><span data-stu-id="85263-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85263-133">id</span><span class="sxs-lookup"><span data-stu-id="85263-133">id</span></span>|<span data-ttu-id="85263-134">String</span><span class="sxs-lookup"><span data-stu-id="85263-134">String</span></span>|<span data-ttu-id="85263-135">TEM 合作伙伴的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="85263-135">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="85263-136">displayName</span><span class="sxs-lookup"><span data-stu-id="85263-136">displayName</span></span>|<span data-ttu-id="85263-137">String</span><span class="sxs-lookup"><span data-stu-id="85263-137">String</span></span>|<span data-ttu-id="85263-138">TEM 合作伙伴的显示名称。</span><span class="sxs-lookup"><span data-stu-id="85263-138">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="85263-139">url</span><span class="sxs-lookup"><span data-stu-id="85263-139">url</span></span>|<span data-ttu-id="85263-140">String</span><span class="sxs-lookup"><span data-stu-id="85263-140">String</span></span>|<span data-ttu-id="85263-141">TEM 合作伙伴的管理控制面板的 URL，管理员可以在其中配置其 TEM 服务。</span><span class="sxs-lookup"><span data-stu-id="85263-141">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="85263-142">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="85263-142">appAuthorized</span></span>|<span data-ttu-id="85263-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="85263-143">Boolean</span></span>|<span data-ttu-id="85263-144">是否已授权合作伙伴的 AAD 应用访问 Intune。</span><span class="sxs-lookup"><span data-stu-id="85263-144">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="85263-145">enabled</span><span class="sxs-lookup"><span data-stu-id="85263-145">enabled</span></span>|<span data-ttu-id="85263-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="85263-146">Boolean</span></span>|<span data-ttu-id="85263-147">当前是启用还是禁用了 Intune 的 TEM 服务连接。</span><span class="sxs-lookup"><span data-stu-id="85263-147">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="85263-148">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="85263-148">lastConnectionDateTime</span></span>|<span data-ttu-id="85263-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85263-149">DateTimeOffset</span></span>|<span data-ttu-id="85263-150">TEM 合作伙伴发送到 Intune 的上一个请求的时间戳。</span><span class="sxs-lookup"><span data-stu-id="85263-150">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85263-151">关系</span><span class="sxs-lookup"><span data-stu-id="85263-151">Relationships</span></span>
<span data-ttu-id="85263-152">无</span><span class="sxs-lookup"><span data-stu-id="85263-152">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85263-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85263-153">JSON Representation</span></span>
<span data-ttu-id="85263-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85263-154">Here is a JSON representation of the resource.</span></span>
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





