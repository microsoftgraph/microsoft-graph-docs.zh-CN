---
title: deviceManagementDomainJoinConnector 资源类型
description: 域加入连接器是负责分配（和删除）计算机帐户 blob 的连接器
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 145b55fa4aa7e9e03823e0b1cabacb7c00db7f11
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524214"
---
# <a name="devicemanagementdomainjoinconnector-resource-type"></a><span data-ttu-id="c3cc4-103">deviceManagementDomainJoinConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3cc4-103">deviceManagementDomainJoinConnector resource type</span></span>

<span data-ttu-id="c3cc4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c3cc4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3cc4-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3cc4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3cc4-107">域加入连接器是负责分配（和删除）计算机帐户 blob 的连接器</span><span class="sxs-lookup"><span data-stu-id="c3cc4-107">A Domain Join Connector is a connector that is responsible to allocate (and delete) machine account blobs</span></span>

## <a name="methods"></a><span data-ttu-id="c3cc4-108">方法</span><span class="sxs-lookup"><span data-stu-id="c3cc4-108">Methods</span></span>
|<span data-ttu-id="c3cc4-109">方法</span><span class="sxs-lookup"><span data-stu-id="c3cc4-109">Method</span></span>|<span data-ttu-id="c3cc4-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c3cc4-110">Return Type</span></span>|<span data-ttu-id="c3cc4-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3cc4-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c3cc4-112">列出 deviceManagementDomainJoinConnectors</span><span class="sxs-lookup"><span data-stu-id="c3cc4-112">List deviceManagementDomainJoinConnectors</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-list.md)|<span data-ttu-id="c3cc4-113">[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="c3cc4-113">[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) collection</span></span>|<span data-ttu-id="c3cc4-114">列出[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-114">List properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) objects.</span></span>|
|[<span data-ttu-id="c3cc4-115">获取 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-115">Get deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-get.md)|[<span data-ttu-id="c3cc4-116">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-116">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="c3cc4-117">读取[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-117">Read properties and relationships of the [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="c3cc4-118">创建 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-118">Create deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-create.md)|[<span data-ttu-id="c3cc4-119">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-119">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="c3cc4-120">创建新的[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-120">Create a new [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|
|[<span data-ttu-id="c3cc4-121">删除 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-121">Delete deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-delete.md)|<span data-ttu-id="c3cc4-122">无</span><span class="sxs-lookup"><span data-stu-id="c3cc4-122">None</span></span>|<span data-ttu-id="c3cc4-123">删除[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-123">Deletes a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md).</span></span>|
|[<span data-ttu-id="c3cc4-124">更新 deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-124">Update deviceManagementDomainJoinConnector</span></span>](../api/intune-odj-devicemanagementdomainjoinconnector-update.md)|[<span data-ttu-id="c3cc4-125">deviceManagementDomainJoinConnector</span><span class="sxs-lookup"><span data-stu-id="c3cc4-125">deviceManagementDomainJoinConnector</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnector.md)|<span data-ttu-id="c3cc4-126">更新[deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-126">Update the properties of a [deviceManagementDomainJoinConnector](../resources/intune-odj-devicemanagementdomainjoinconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c3cc4-127">属性</span><span class="sxs-lookup"><span data-stu-id="c3cc4-127">Properties</span></span>
|<span data-ttu-id="c3cc4-128">属性</span><span class="sxs-lookup"><span data-stu-id="c3cc4-128">Property</span></span>|<span data-ttu-id="c3cc4-129">类型</span><span class="sxs-lookup"><span data-stu-id="c3cc4-129">Type</span></span>|<span data-ttu-id="c3cc4-130">说明</span><span class="sxs-lookup"><span data-stu-id="c3cc4-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3cc4-131">id</span><span class="sxs-lookup"><span data-stu-id="c3cc4-131">id</span></span>|<span data-ttu-id="c3cc4-132">String</span><span class="sxs-lookup"><span data-stu-id="c3cc4-132">String</span></span>|<span data-ttu-id="c3cc4-133">代表连接器的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-133">Unique identifier to represent a connector.</span></span>|
|<span data-ttu-id="c3cc4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c3cc4-134">displayName</span></span>|<span data-ttu-id="c3cc4-135">字符串</span><span class="sxs-lookup"><span data-stu-id="c3cc4-135">String</span></span>|<span data-ttu-id="c3cc4-136">连接器显示名称。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-136">The connector display name.</span></span>|
|<span data-ttu-id="c3cc4-137">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="c3cc4-137">lastConnectionDateTime</span></span>|<span data-ttu-id="c3cc4-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3cc4-138">DateTimeOffset</span></span>|<span data-ttu-id="c3cc4-139">上次联系 Intune 的时间连接器。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-139">Last time connector contacted Intune.</span></span>|
|<span data-ttu-id="c3cc4-140">state</span><span class="sxs-lookup"><span data-stu-id="c3cc4-140">state</span></span>|[<span data-ttu-id="c3cc4-141">deviceManagementDomainJoinConnectorState</span><span class="sxs-lookup"><span data-stu-id="c3cc4-141">deviceManagementDomainJoinConnectorState</span></span>](../resources/intune-odj-devicemanagementdomainjoinconnectorstate.md)|<span data-ttu-id="c3cc4-142">连接器状态。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-142">The connector state.</span></span> <span data-ttu-id="c3cc4-143">可取值为：`active`、`error`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-143">Possible values are: `active`, `error`, `inactive`.</span></span>|
|<span data-ttu-id="c3cc4-144">version</span><span class="sxs-lookup"><span data-stu-id="c3cc4-144">version</span></span>|<span data-ttu-id="c3cc4-145">String</span><span class="sxs-lookup"><span data-stu-id="c3cc4-145">String</span></span>|<span data-ttu-id="c3cc4-146">连接器的版本。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-146">The version of the connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3cc4-147">关系</span><span class="sxs-lookup"><span data-stu-id="c3cc4-147">Relationships</span></span>
<span data-ttu-id="c3cc4-148">无</span><span class="sxs-lookup"><span data-stu-id="c3cc4-148">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3cc4-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3cc4-149">JSON Representation</span></span>
<span data-ttu-id="c3cc4-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3cc4-150">Here is a JSON representation of the resource.</span></span>
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



