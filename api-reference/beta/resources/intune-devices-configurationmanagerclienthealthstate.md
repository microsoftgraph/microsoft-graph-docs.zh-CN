---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端运行状况
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1c1c707d118b666f52e8a898cd0ad258c5cc8308
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43465035"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="ea1a3-103">configurationManagerClientHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="ea1a3-103">configurationManagerClientHealthState resource type</span></span>

<span data-ttu-id="ea1a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea1a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea1a3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea1a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea1a3-107">配置管理器客户端运行状况</span><span class="sxs-lookup"><span data-stu-id="ea1a3-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="ea1a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea1a3-108">Properties</span></span>
|<span data-ttu-id="ea1a3-109">属性</span><span class="sxs-lookup"><span data-stu-id="ea1a3-109">Property</span></span>|<span data-ttu-id="ea1a3-110">类型</span><span class="sxs-lookup"><span data-stu-id="ea1a3-110">Type</span></span>|<span data-ttu-id="ea1a3-111">说明</span><span class="sxs-lookup"><span data-stu-id="ea1a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea1a3-112">state</span><span class="sxs-lookup"><span data-stu-id="ea1a3-112">state</span></span>|[<span data-ttu-id="ea1a3-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="ea1a3-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="ea1a3-114">当前配置管理器客户端状态。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-114">Current configuration manager client state.</span></span> <span data-ttu-id="ea1a3-115">可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="ea1a3-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="ea1a3-116">errorCode</span></span>|<span data-ttu-id="ea1a3-117">Int32</span><span class="sxs-lookup"><span data-stu-id="ea1a3-117">Int32</span></span>|<span data-ttu-id="ea1a3-118">失败状态的错误代码。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-118">Error code for failed state.</span></span>|
|<span data-ttu-id="ea1a3-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ea1a3-119">lastSyncDateTime</span></span>|<span data-ttu-id="ea1a3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ea1a3-120">DateTimeOffset</span></span>|<span data-ttu-id="ea1a3-121">与 configuration manager 管理点进行上一次同步的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-121">Datetime for last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea1a3-122">关系</span><span class="sxs-lookup"><span data-stu-id="ea1a3-122">Relationships</span></span>
<span data-ttu-id="ea1a3-123">无</span><span class="sxs-lookup"><span data-stu-id="ea1a3-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea1a3-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ea1a3-124">JSON Representation</span></span>
<span data-ttu-id="ea1a3-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea1a3-125">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientHealthState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientHealthState",
  "state": "String",
  "errorCode": 1024,
  "lastSyncDateTime": "String (timestamp)"
}
```



