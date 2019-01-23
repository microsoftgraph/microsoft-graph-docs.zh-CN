---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端健康状态
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 55ba2b24df0d1d4c278f4785a310237c9c32cd9b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425825"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="8663d-103">configurationManagerClientHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="8663d-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="8663d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8663d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8663d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8663d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8663d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8663d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8663d-107">配置管理器客户端健康状态</span><span class="sxs-lookup"><span data-stu-id="8663d-107">Configuration manager client health state</span></span>

## <a name="properties"></a><span data-ttu-id="8663d-108">属性</span><span class="sxs-lookup"><span data-stu-id="8663d-108">Properties</span></span>
|<span data-ttu-id="8663d-109">属性</span><span class="sxs-lookup"><span data-stu-id="8663d-109">Property</span></span>|<span data-ttu-id="8663d-110">类型</span><span class="sxs-lookup"><span data-stu-id="8663d-110">Type</span></span>|<span data-ttu-id="8663d-111">说明</span><span class="sxs-lookup"><span data-stu-id="8663d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8663d-112">state</span><span class="sxs-lookup"><span data-stu-id="8663d-112">state</span></span>|[<span data-ttu-id="8663d-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="8663d-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="8663d-114">当前配置管理器客户端状态。</span><span class="sxs-lookup"><span data-stu-id="8663d-114">Current configuration manager client state.</span></span> <span data-ttu-id="8663d-115">可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。</span><span class="sxs-lookup"><span data-stu-id="8663d-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="8663d-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="8663d-116">errorCode</span></span>|<span data-ttu-id="8663d-117">Int32</span><span class="sxs-lookup"><span data-stu-id="8663d-117">Int32</span></span>|<span data-ttu-id="8663d-118">失败的状态的错误代码。</span><span class="sxs-lookup"><span data-stu-id="8663d-118">Error code for failed state.</span></span>|
|<span data-ttu-id="8663d-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="8663d-119">lastSyncDateTime</span></span>|<span data-ttu-id="8663d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8663d-120">DateTimeOffset</span></span>|<span data-ttu-id="8663d-121">指向与配置管理器管理的 Datetime fo 上次同步。</span><span class="sxs-lookup"><span data-stu-id="8663d-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8663d-122">关系</span><span class="sxs-lookup"><span data-stu-id="8663d-122">Relationships</span></span>
<span data-ttu-id="8663d-123">无</span><span class="sxs-lookup"><span data-stu-id="8663d-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8663d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8663d-124">JSON Representation</span></span>
<span data-ttu-id="8663d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8663d-125">Here is a JSON representation of the resource.</span></span>
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




