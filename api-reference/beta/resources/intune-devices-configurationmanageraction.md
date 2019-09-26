---
title: configurationManagerAction 资源类型
description: Action triggerConfigurationManagerAction 的参数
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ff71bc6b4094543e3da6d22639014f595a86ce7d
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37200001"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="fc473-103">configurationManagerAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="fc473-103">configurationManagerAction resource type</span></span>

> <span data-ttu-id="fc473-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc473-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc473-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc473-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc473-106">Action triggerConfigurationManagerAction 的参数</span><span class="sxs-lookup"><span data-stu-id="fc473-106">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="fc473-107">属性</span><span class="sxs-lookup"><span data-stu-id="fc473-107">Properties</span></span>
|<span data-ttu-id="fc473-108">属性</span><span class="sxs-lookup"><span data-stu-id="fc473-108">Property</span></span>|<span data-ttu-id="fc473-109">类型</span><span class="sxs-lookup"><span data-stu-id="fc473-109">Type</span></span>|<span data-ttu-id="fc473-110">说明</span><span class="sxs-lookup"><span data-stu-id="fc473-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc473-111">action</span><span class="sxs-lookup"><span data-stu-id="fc473-111">action</span></span>|[<span data-ttu-id="fc473-112">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="fc473-112">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="fc473-113">要在 Configuration Manager 客户端上触发的操作类型。</span><span class="sxs-lookup"><span data-stu-id="fc473-113">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="fc473-114">可取值为：`refreshMachinePolicy`、`refreshUserPolicy`、`wakeUpClient`、`appEvaluation`。</span><span class="sxs-lookup"><span data-stu-id="fc473-114">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fc473-115">关系</span><span class="sxs-lookup"><span data-stu-id="fc473-115">Relationships</span></span>
<span data-ttu-id="fc473-116">无</span><span class="sxs-lookup"><span data-stu-id="fc473-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fc473-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fc473-117">JSON Representation</span></span>
<span data-ttu-id="fc473-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc473-118">Here is a JSON representation of the resource.</span></span>
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



