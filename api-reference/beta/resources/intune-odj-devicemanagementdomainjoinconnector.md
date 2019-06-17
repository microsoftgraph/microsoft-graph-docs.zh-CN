---
title: deviceManagementDomainJoinConnector 资源类型
description: 域加入连接器是负责分配 (和删除) 计算机帐户 blob 的连接器
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0537d38d87a2cb574ca8984f895ed3796c33703a
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001921"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a><span data-ttu-id="d48ad-103">deviceManagementDomainJoinConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="d48ad-103">deviceManagementDomainJoinConnector resource type</span></span>

> <span data-ttu-id="d48ad-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d48ad-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d48ad-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d48ad-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d48ad-106">域加入连接器是负责分配 (和删除) 计算机帐户 blob 的连接器</span><span class="sxs-lookup"><span data-stu-id="d48ad-106">A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs</span></span>

## <a name="methods"></a><span data-ttu-id="d48ad-107">方法</span><span class="sxs-lookup"><span data-stu-id="d48ad-107">Methods</span></span>
|<span data-ttu-id="d48ad-108">方法</span><span class="sxs-lookup"><span data-stu-id="d48ad-108">Method</span></span>|<span data-ttu-id="d48ad-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="d48ad-109">Return Type</span></span>|<span data-ttu-id="d48ad-110">说明</span><span class="sxs-lookup"><span data-stu-id="d48ad-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d48ad-111">列出 deviceManagementDomainJoinConnectors</span><span class="sxs-lookup"><span data-stu-id="d48ad-111">List deviceManagementDomainJoinConnectors</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|<span data-ttu-id="d48ad-112">[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="d48ad-112">[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) collection</span></span>|<span data-ttu-id="d48ad-113">列出[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d48ad-113">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>|
|[<span data-ttu-id="d48ad-114">获取 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-114">Get deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[<span data-ttu-id="d48ad-115">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-115">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="d48ad-116">读取[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d48ad-116">Read properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="d48ad-117">创建 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-117">Create deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[<span data-ttu-id="d48ad-118">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-118">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="d48ad-119">创建新的[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d48ad-119">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="d48ad-120">删除 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-120">Delete deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|<span data-ttu-id="d48ad-121">无</span><span class="sxs-lookup"><span data-stu-id="d48ad-121">None</span></span>|<span data-ttu-id="d48ad-122">删除[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="d48ad-122">Deletes a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>|
|[<span data-ttu-id="d48ad-123">更新 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-123">Update deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[<span data-ttu-id="d48ad-124">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="d48ad-124">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="d48ad-125">更新[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d48ad-125">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d48ad-126">属性</span><span class="sxs-lookup"><span data-stu-id="d48ad-126">Properties</span></span>
|<span data-ttu-id="d48ad-127">属性</span><span class="sxs-lookup"><span data-stu-id="d48ad-127">Property</span></span>|<span data-ttu-id="d48ad-128">类型</span><span class="sxs-lookup"><span data-stu-id="d48ad-128">Type</span></span>|<span data-ttu-id="d48ad-129">说明</span><span class="sxs-lookup"><span data-stu-id="d48ad-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d48ad-130">id</span><span class="sxs-lookup"><span data-stu-id="d48ad-130">id</span></span>|<span data-ttu-id="d48ad-131">String</span><span class="sxs-lookup"><span data-stu-id="d48ad-131">String</span></span>|<span data-ttu-id="d48ad-132">代表连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d48ad-132">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="d48ad-133">displayName</span><span class="sxs-lookup"><span data-stu-id="d48ad-133">displayName</span></span>|<span data-ttu-id="d48ad-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d48ad-134">String</span></span>|<span data-ttu-id="d48ad-135">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="d48ad-135">The connector display name.</span></span>|
|<span data-ttu-id="d48ad-136">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d48ad-136">lastConnectionDateTime</span></span>|<span data-ttu-id="d48ad-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d48ad-137">DateTimeOffset</span></span>|<span data-ttu-id="d48ad-138">上次联系 Intune 的时间连接器。</span><span class="sxs-lookup"><span data-stu-id="d48ad-138">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="d48ad-139">state</span><span class="sxs-lookup"><span data-stu-id="d48ad-139">state</span></span>|[<span data-ttu-id="d48ad-140">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="d48ad-140">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="d48ad-141">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="d48ad-141">The connector state.</span></span> <span data-ttu-id="d48ad-142">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="d48ad-142">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="d48ad-143">version</span><span class="sxs-lookup"><span data-stu-id="d48ad-143">version</span></span>|<span data-ttu-id="d48ad-144">String</span><span class="sxs-lookup"><span data-stu-id="d48ad-144">String</span></span>|<span data-ttu-id="d48ad-145">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="d48ad-145">The version of the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d48ad-146">关系</span><span class="sxs-lookup"><span data-stu-id="d48ad-146">Relationships</span></span>
<span data-ttu-id="d48ad-147">无</span><span class="sxs-lookup"><span data-stu-id="d48ad-147">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d48ad-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d48ad-148">JSON Representation</span></span>
<span data-ttu-id="d48ad-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d48ad-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementDomainJoinConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementDomainJoinConnector",
  "id": "String (identifier)",
  "displayName": "String",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "version": "String"
}
```





