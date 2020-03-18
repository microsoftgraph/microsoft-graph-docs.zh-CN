---
title: configurationManagerAction 资源类型
description: Action triggerConfigurationManagerAction 的参数
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 04d78d751f6cdd2978aa9cc65942acf312482202
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785096"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="512c4-103">configurationManagerAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="512c4-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="512c4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="512c4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="512c4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="512c4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="512c4-106">Action triggerConfigurationManagerAction 的参数</span><span class="sxs-lookup"><span data-stu-id="512c4-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="512c4-107">属性</span><span class="sxs-lookup"><span data-stu-id="512c4-107">Properties</span></span>
|<span data-ttu-id="512c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="512c4-108">Property</span></span>|<span data-ttu-id="512c4-109">类型</span><span class="sxs-lookup"><span data-stu-id="512c4-109">Type</span></span>|<span data-ttu-id="512c4-110">说明</span><span class="sxs-lookup"><span data-stu-id="512c4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="512c4-111">action</span><span class="sxs-lookup"><span data-stu-id="512c4-111">action</span></span>|[<span data-ttu-id="512c4-112">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="512c4-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="512c4-113">要在 Configuration Manager 客户端上触发的操作类型。</span><span class="sxs-lookup"><span data-stu-id="512c4-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="512c4-114">可取值为：`refreshMachinePolicy`、`refreshUserPolicy`、`wakeUpClient`、`appEvaluation`。</span><span class="sxs-lookup"><span data-stu-id="512c4-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="512c4-115">关系</span><span class="sxs-lookup"><span data-stu-id="512c4-115">Relationships</span></span>
<span data-ttu-id="512c4-116">无</span><span class="sxs-lookup"><span data-stu-id="512c4-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="512c4-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="512c4-117">JSON Representation</span></span>
<span data-ttu-id="512c4-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="512c4-118">Here is a JSON representation of the resource.</span></span>
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



