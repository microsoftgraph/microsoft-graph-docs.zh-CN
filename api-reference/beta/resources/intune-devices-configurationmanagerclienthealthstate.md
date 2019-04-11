---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端运行状况
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2a04b8cf7520425527e118fcc9db00461c4edda
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31797737"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="b92c5-103">configurationManagerClientHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b92c5-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="b92c5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b92c5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b92c5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b92c5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b92c5-106">配置管理器客户端运行状况</span><span class="sxs-lookup"><span data-stu-id="b92c5-106">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="b92c5-107">属性</span><span class="sxs-lookup"><span data-stu-id="b92c5-107">Properties</span></span>
|<span data-ttu-id="b92c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="b92c5-108">Property</span></span>|<span data-ttu-id="b92c5-109">类型</span><span class="sxs-lookup"><span data-stu-id="b92c5-109">Type</span></span>|<span data-ttu-id="b92c5-110">说明</span><span class="sxs-lookup"><span data-stu-id="b92c5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b92c5-111">state</span><span class="sxs-lookup"><span data-stu-id="b92c5-111">state</span></span>|[<span data-ttu-id="b92c5-112">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="b92c5-112">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="b92c5-113">当前配置管理器客户端状态。</span><span class="sxs-lookup"><span data-stu-id="b92c5-113">Current configuration manager client state.</span></span> <span data-ttu-id="b92c5-114">可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。</span><span class="sxs-lookup"><span data-stu-id="b92c5-114">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="b92c5-115">errorCode</span><span class="sxs-lookup"><span data-stu-id="b92c5-115">errorCode</span></span>|<span data-ttu-id="b92c5-116">Int32</span><span class="sxs-lookup"><span data-stu-id="b92c5-116">Int32</span></span>|<span data-ttu-id="b92c5-117">失败状态的错误代码。</span><span class="sxs-lookup"><span data-stu-id="b92c5-117">Error code for failed state.</span></span>|
|<span data-ttu-id="b92c5-118">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="b92c5-118">lastSyncDateTime</span></span>|<span data-ttu-id="b92c5-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b92c5-119">DateTimeOffset</span></span>|<span data-ttu-id="b92c5-120">上次与 configuration manager 管理点同步的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b92c5-120">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b92c5-121">关系</span><span class="sxs-lookup"><span data-stu-id="b92c5-121">Relationships</span></span>
<span data-ttu-id="b92c5-122">无</span><span class="sxs-lookup"><span data-stu-id="b92c5-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b92c5-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b92c5-123">JSON Representation</span></span>
<span data-ttu-id="b92c5-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b92c5-124">Here is a JSON representation of the resource.</span></span>
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





