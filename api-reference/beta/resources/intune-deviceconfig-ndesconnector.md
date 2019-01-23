---
title: ndesConnector 资源类型
description: 代表 OnPrem Ndes 连接器的实体。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b504173c0a56e15fd2a4ba09ce50beeabbb20edc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411146"
---
# <a name="ndesconnector-resource-type"></a><span data-ttu-id="d2b25-103">ndesConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="d2b25-103">ndesConnector resource type</span></span>

> <span data-ttu-id="d2b25-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d2b25-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d2b25-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d2b25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d2b25-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d2b25-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2b25-107">代表 OnPrem Ndes 连接器的实体。</span><span class="sxs-lookup"><span data-stu-id="d2b25-107">Entity which represents an OnPrem Ndes connector.</span></span>

## <a name="methods"></a><span data-ttu-id="d2b25-108">方法</span><span class="sxs-lookup"><span data-stu-id="d2b25-108">Methods</span></span>
|<span data-ttu-id="d2b25-109">方法</span><span class="sxs-lookup"><span data-stu-id="d2b25-109">Method</span></span>|<span data-ttu-id="d2b25-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="d2b25-110">Return Type</span></span>|<span data-ttu-id="d2b25-111">说明</span><span class="sxs-lookup"><span data-stu-id="d2b25-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2b25-112">列表 ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="d2b25-112">List ndesConnectors</span></span>](../api/intune-deviceconfig-ndesconnector-list.md)|<span data-ttu-id="d2b25-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="d2b25-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) collection</span></span>|<span data-ttu-id="d2b25-114">列出属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="d2b25-114">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>|
|[<span data-ttu-id="d2b25-115">获取 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-115">Get ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-get.md)|[<span data-ttu-id="d2b25-116">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-116">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d2b25-117">读取属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="d2b25-117">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="d2b25-118">创建 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-118">Create ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-create.md)|[<span data-ttu-id="d2b25-119">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-119">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d2b25-120">创建新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2b25-120">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="d2b25-121">删除 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-121">Delete ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-delete.md)|<span data-ttu-id="d2b25-122">无</span><span class="sxs-lookup"><span data-stu-id="d2b25-122">None</span></span>|<span data-ttu-id="d2b25-123">删除[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="d2b25-123">Deletes a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>|
|[<span data-ttu-id="d2b25-124">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-124">Update ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-update.md)|[<span data-ttu-id="d2b25-125">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="d2b25-125">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="d2b25-126">更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d2b25-126">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d2b25-127">属性</span><span class="sxs-lookup"><span data-stu-id="d2b25-127">Properties</span></span>
|<span data-ttu-id="d2b25-128">属性</span><span class="sxs-lookup"><span data-stu-id="d2b25-128">Property</span></span>|<span data-ttu-id="d2b25-129">类型</span><span class="sxs-lookup"><span data-stu-id="d2b25-129">Type</span></span>|<span data-ttu-id="d2b25-130">说明</span><span class="sxs-lookup"><span data-stu-id="d2b25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2b25-131">id</span><span class="sxs-lookup"><span data-stu-id="d2b25-131">id</span></span>|<span data-ttu-id="d2b25-132">String</span><span class="sxs-lookup"><span data-stu-id="d2b25-132">String</span></span>|<span data-ttu-id="d2b25-133">NDES 连接符的键。</span><span class="sxs-lookup"><span data-stu-id="d2b25-133">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="d2b25-134">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="d2b25-134">lastConnectionDateTime</span></span>|<span data-ttu-id="d2b25-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2b25-135">DateTimeOffset</span></span>|<span data-ttu-id="d2b25-136">Ndes 连接器的最后一个连接时间</span><span class="sxs-lookup"><span data-stu-id="d2b25-136">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="d2b25-137">state</span><span class="sxs-lookup"><span data-stu-id="d2b25-137">state</span></span>|[<span data-ttu-id="d2b25-138">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="d2b25-138">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="d2b25-139">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="d2b25-139">Ndes Connector Status.</span></span> <span data-ttu-id="d2b25-140">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="d2b25-140">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="d2b25-141">displayName</span><span class="sxs-lookup"><span data-stu-id="d2b25-141">displayName</span></span>|<span data-ttu-id="d2b25-142">String</span><span class="sxs-lookup"><span data-stu-id="d2b25-142">String</span></span>|<span data-ttu-id="d2b25-143">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="d2b25-143">The friendly name of the Ndes Connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2b25-144">关系</span><span class="sxs-lookup"><span data-stu-id="d2b25-144">Relationships</span></span>
<span data-ttu-id="d2b25-145">无</span><span class="sxs-lookup"><span data-stu-id="d2b25-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2b25-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d2b25-146">JSON Representation</span></span>
<span data-ttu-id="d2b25-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d2b25-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ndesConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.ndesConnector",
  "id": "String (identifier)",
  "lastConnectionDateTime": "String (timestamp)",
  "state": "String",
  "displayName": "String"
}
```




