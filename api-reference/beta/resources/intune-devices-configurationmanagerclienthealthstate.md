---
title: configurationManagerClientHealthState 资源类型
description: 配置管理器客户端健康状态
author: tfitzmac
ms.openlocfilehash: 8361d74f675cf1eaf70b78e2350aae2fc6e83554
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302784"
---
# <a name="configurationmanagerclienthealthstate-resource-type"></a><span data-ttu-id="60c3d-103">configurationManagerClientHealthState 资源类型</span><span class="sxs-lookup"><span data-stu-id="60c3d-103">configurationManagerClientHealthState resource type</span></span>

> <span data-ttu-id="60c3d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60c3d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60c3d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60c3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60c3d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="60c3d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60c3d-107">配置管理器客户端健康状态</span><span class="sxs-lookup"><span data-stu-id="60c3d-107">Configuration manager client health state</span></span>
## <a name="properties"></a><span data-ttu-id="60c3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="60c3d-108">Properties</span></span>
|<span data-ttu-id="60c3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="60c3d-109">Property</span></span>|<span data-ttu-id="60c3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="60c3d-110">Type</span></span>|<span data-ttu-id="60c3d-111">说明</span><span class="sxs-lookup"><span data-stu-id="60c3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60c3d-112">state</span><span class="sxs-lookup"><span data-stu-id="60c3d-112">state</span></span>|[<span data-ttu-id="60c3d-113">configurationManagerClientState</span><span class="sxs-lookup"><span data-stu-id="60c3d-113">configurationManagerClientState</span></span>](../resources/intune-devices-configurationmanagerclientstate.md)|<span data-ttu-id="60c3d-114">当前配置管理器客户端状态。</span><span class="sxs-lookup"><span data-stu-id="60c3d-114">Current configuration manager client state.</span></span> <span data-ttu-id="60c3d-115">可取值为：`unknown`、`installed`、`healthy`、`installFailed`、`updateFailed`、`communicationError`。</span><span class="sxs-lookup"><span data-stu-id="60c3d-115">Possible values are: `unknown`, `installed`, `healthy`, `installFailed`, `updateFailed`, `communicationError`.</span></span>|
|<span data-ttu-id="60c3d-116">errorCode</span><span class="sxs-lookup"><span data-stu-id="60c3d-116">errorCode</span></span>|<span data-ttu-id="60c3d-117">Int32</span><span class="sxs-lookup"><span data-stu-id="60c3d-117">Int32</span></span>|<span data-ttu-id="60c3d-118">失败的状态的错误代码。</span><span class="sxs-lookup"><span data-stu-id="60c3d-118">Error code for failed state.</span></span>|
|<span data-ttu-id="60c3d-119">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="60c3d-119">lastSyncDateTime</span></span>|<span data-ttu-id="60c3d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60c3d-120">DateTimeOffset</span></span>|<span data-ttu-id="60c3d-121">指向与配置管理器管理的 Datetime fo 上次同步。</span><span class="sxs-lookup"><span data-stu-id="60c3d-121">Datetime fo last sync with configuration manager management point.</span></span>|

## <a name="relationships"></a><span data-ttu-id="60c3d-122">Relationships</span><span class="sxs-lookup"><span data-stu-id="60c3d-122">Relationships</span></span>
<span data-ttu-id="60c3d-123">无</span><span class="sxs-lookup"><span data-stu-id="60c3d-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="60c3d-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60c3d-124">JSON Representation</span></span>
<span data-ttu-id="60c3d-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60c3d-125">Here is a JSON representation of the resource.</span></span>
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





