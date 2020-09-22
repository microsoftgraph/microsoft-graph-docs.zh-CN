---
title: configurationManagerAction 资源类型
description: Action triggerConfigurationManagerAction 的参数
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b16f09234c1c0c90930b99044648aa8d4236a023
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060711"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="62d42-103">configurationManagerAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="62d42-103">configurationManagerAction resource type</span></span>

<span data-ttu-id="62d42-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62d42-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62d42-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62d42-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62d42-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62d42-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62d42-107">Action triggerConfigurationManagerAction 的参数</span><span class="sxs-lookup"><span data-stu-id="62d42-107">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="62d42-108">属性</span><span class="sxs-lookup"><span data-stu-id="62d42-108">Properties</span></span>
|<span data-ttu-id="62d42-109">属性</span><span class="sxs-lookup"><span data-stu-id="62d42-109">Property</span></span>|<span data-ttu-id="62d42-110">类型</span><span class="sxs-lookup"><span data-stu-id="62d42-110">Type</span></span>|<span data-ttu-id="62d42-111">说明</span><span class="sxs-lookup"><span data-stu-id="62d42-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62d42-112">action</span><span class="sxs-lookup"><span data-stu-id="62d42-112">action</span></span>|[<span data-ttu-id="62d42-113">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="62d42-113">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="62d42-114">要在 Configuration Manager 客户端上触发的操作类型。</span><span class="sxs-lookup"><span data-stu-id="62d42-114">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="62d42-115">可取值为：`refreshMachinePolicy`、`refreshUserPolicy`、`wakeUpClient`、`appEvaluation`。</span><span class="sxs-lookup"><span data-stu-id="62d42-115">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62d42-116">关系</span><span class="sxs-lookup"><span data-stu-id="62d42-116">Relationships</span></span>
<span data-ttu-id="62d42-117">无</span><span class="sxs-lookup"><span data-stu-id="62d42-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62d42-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62d42-118">JSON Representation</span></span>
<span data-ttu-id="62d42-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62d42-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerAction",
  "action": "String"
}
```






