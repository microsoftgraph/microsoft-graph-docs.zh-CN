---
title: ndesConnector 资源类型
description: 代表 OnPrem Ndes 连接器的实体。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 582d49ccd9a5d61c144e3ef915994302515dbe40
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884915"
---
# <a name="ndesconnector-resource-type"></a><span data-ttu-id="84c2a-103">ndesConnector 资源类型</span><span class="sxs-lookup"><span data-stu-id="84c2a-103">ndesConnector resource type</span></span>

> <span data-ttu-id="84c2a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="84c2a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84c2a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84c2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84c2a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="84c2a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84c2a-107">代表 OnPrem Ndes 连接器的实体。</span><span class="sxs-lookup"><span data-stu-id="84c2a-107">Entity which represents an OnPrem Ndes connector.</span></span>
## <a name="methods"></a><span data-ttu-id="84c2a-108">方法</span><span class="sxs-lookup"><span data-stu-id="84c2a-108">Methods</span></span>
|<span data-ttu-id="84c2a-109">方法</span><span class="sxs-lookup"><span data-stu-id="84c2a-109">Method</span></span>|<span data-ttu-id="84c2a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="84c2a-110">Return Type</span></span>|<span data-ttu-id="84c2a-111">说明</span><span class="sxs-lookup"><span data-stu-id="84c2a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84c2a-112">列表 ndesConnectors</span><span class="sxs-lookup"><span data-stu-id="84c2a-112">List ndesConnectors</span></span>](../api/intune-deviceconfig-ndesconnector-list.md)|<span data-ttu-id="84c2a-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)集合</span><span class="sxs-lookup"><span data-stu-id="84c2a-113">[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) collection</span></span>|<span data-ttu-id="84c2a-114">列出属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="84c2a-114">List properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) objects.</span></span>|
|[<span data-ttu-id="84c2a-115">获取 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-115">Get ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-get.md)|[<span data-ttu-id="84c2a-116">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-116">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="84c2a-117">读取属性和[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="84c2a-117">Read properties and relationships of the [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="84c2a-118">创建 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-118">Create ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-create.md)|[<span data-ttu-id="84c2a-119">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-119">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="84c2a-120">创建新的[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84c2a-120">Create a new [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|
|[<span data-ttu-id="84c2a-121">删除 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-121">Delete ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-delete.md)|<span data-ttu-id="84c2a-122">无</span><span class="sxs-lookup"><span data-stu-id="84c2a-122">None</span></span>|<span data-ttu-id="84c2a-123">删除[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)。</span><span class="sxs-lookup"><span data-stu-id="84c2a-123">Deletes a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md).</span></span>|
|[<span data-ttu-id="84c2a-124">更新 ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-124">Update ndesConnector</span></span>](../api/intune-deviceconfig-ndesconnector-update.md)|[<span data-ttu-id="84c2a-125">ndesConnector</span><span class="sxs-lookup"><span data-stu-id="84c2a-125">ndesConnector</span></span>](../resources/intune-deviceconfig-ndesconnector.md)|<span data-ttu-id="84c2a-126">更新[ndesConnector](../resources/intune-deviceconfig-ndesconnector.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84c2a-126">Update the properties of a [ndesConnector](../resources/intune-deviceconfig-ndesconnector.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84c2a-127">属性</span><span class="sxs-lookup"><span data-stu-id="84c2a-127">Properties</span></span>
|<span data-ttu-id="84c2a-128">属性</span><span class="sxs-lookup"><span data-stu-id="84c2a-128">Property</span></span>|<span data-ttu-id="84c2a-129">类型</span><span class="sxs-lookup"><span data-stu-id="84c2a-129">Type</span></span>|<span data-ttu-id="84c2a-130">说明</span><span class="sxs-lookup"><span data-stu-id="84c2a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84c2a-131">id</span><span class="sxs-lookup"><span data-stu-id="84c2a-131">id</span></span>|<span data-ttu-id="84c2a-132">字符串</span><span class="sxs-lookup"><span data-stu-id="84c2a-132">String</span></span>|<span data-ttu-id="84c2a-133">NDES 连接符的键。</span><span class="sxs-lookup"><span data-stu-id="84c2a-133">The key of the NDES Connector.</span></span>|
|<span data-ttu-id="84c2a-134">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="84c2a-134">lastConnectionDateTime</span></span>|<span data-ttu-id="84c2a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84c2a-135">DateTimeOffset</span></span>|<span data-ttu-id="84c2a-136">Ndes 连接器的最后一个连接时间</span><span class="sxs-lookup"><span data-stu-id="84c2a-136">Last connection time for the Ndes Connector</span></span>|
|<span data-ttu-id="84c2a-137">state</span><span class="sxs-lookup"><span data-stu-id="84c2a-137">state</span></span>|[<span data-ttu-id="84c2a-138">ndesConnectorState</span><span class="sxs-lookup"><span data-stu-id="84c2a-138">ndesConnectorState</span></span>](../resources/intune-deviceconfig-ndesconnectorstate.md)|<span data-ttu-id="84c2a-139">Ndes 连接器状态。</span><span class="sxs-lookup"><span data-stu-id="84c2a-139">Ndes Connector Status.</span></span> <span data-ttu-id="84c2a-140">可取值为：`none`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="84c2a-140">Possible values are: `none`, `active`, `inactive`.</span></span>|
|<span data-ttu-id="84c2a-141">displayName</span><span class="sxs-lookup"><span data-stu-id="84c2a-141">displayName</span></span>|<span data-ttu-id="84c2a-142">字符串</span><span class="sxs-lookup"><span data-stu-id="84c2a-142">String</span></span>|<span data-ttu-id="84c2a-143">Ndes 连接器的友好名称。</span><span class="sxs-lookup"><span data-stu-id="84c2a-143">The friendly name of the Ndes Connector.</span></span>|

## <a name="relationships"></a><span data-ttu-id="84c2a-144">Relationships</span><span class="sxs-lookup"><span data-stu-id="84c2a-144">Relationships</span></span>
<span data-ttu-id="84c2a-145">无</span><span class="sxs-lookup"><span data-stu-id="84c2a-145">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="84c2a-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84c2a-146">JSON Representation</span></span>
<span data-ttu-id="84c2a-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84c2a-147">Here is a JSON representation of the resource.</span></span>
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





