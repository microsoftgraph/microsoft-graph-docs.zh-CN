---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端健康状态
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d202b5f672977e8bb1a5fe05ba56937005825ff
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27981740"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="d39e8-103">configurationManagerClientHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="d39e8-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="d39e8-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d39e8-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d39e8-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d39e8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d39e8-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d39e8-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d39e8-107">配置管理器客户端健康状态</span><span class="sxs-lookup"><span data-stu-id="d39e8-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="d39e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="d39e8-108">Properties</span></span>
|<span data-ttu-id="d39e8-109">属性</span><span class="sxs-lookup"><span data-stu-id="d39e8-109">Property</span></span>|<span data-ttu-id="d39e8-110">类型</span><span class="sxs-lookup"><span data-stu-id="d39e8-110">Type</span></span>|<span data-ttu-id="d39e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="d39e8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d39e8-112">state</span><span class="sxs-lookup"><span data-stu-id="d39e8-112">state</span></span>|[<span data-ttu-id="d39e8-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="d39e8-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="d39e8-114">当前配置管理器客户端状态。</span><span class="sxs-lookup"><span data-stu-id="d39e8-114">Current configuration manager client state.</span></span> <span data-ttu-id="d39e8-115">可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。</span><span class="sxs-lookup"><span data-stu-id="d39e8-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="d39e8-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="d39e8-116">errorCode</span></span>|<span data-ttu-id="d39e8-117">Int32</span><span class="sxs-lookup"><span data-stu-id="d39e8-117">Int32</span></span>|<span data-ttu-id="d39e8-118">失败的状态的错误代码。</span><span class="sxs-lookup"><span data-stu-id="d39e8-118">Error code for failed state.</span></span>|
|<span data-ttu-id="d39e8-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d39e8-119">lastSyncDateTime</span></span>|<span data-ttu-id="d39e8-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d39e8-120">DateTimeOffset</span></span>|<span data-ttu-id="d39e8-121">指向与配置管理器管理的 Datetime fo 上次同步。</span><span class="sxs-lookup"><span data-stu-id="d39e8-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d39e8-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="d39e8-122">Relationships</span></span>
<span data-ttu-id="d39e8-123">无</span><span class="sxs-lookup"><span data-stu-id="d39e8-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d39e8-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d39e8-124">JSON Representation</span></span>
<span data-ttu-id="d39e8-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d39e8-125">Here is a JSON representation of the resource.</span></span>
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





