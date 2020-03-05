---
title: configurationManagerAction 资源类型
description: Action triggerConfigurationManagerAction 的参数
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 867479fea3f795bc8fbe143a9db054847b79e0d1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528687"
---
# <a name="configurationmanageraction-resource-type"></a><span data-ttu-id="42fd2-103">configurationManagerAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="42fd2-103">configurationManagerAction resource type</span></span>

<span data-ttu-id="42fd2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="42fd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="42fd2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="42fd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="42fd2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="42fd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="42fd2-107">Action triggerConfigurationManagerAction 的参数</span><span class="sxs-lookup"><span data-stu-id="42fd2-107">Parameter for action triggerConfigurationManagerAction</span></span>

## <a name="properties"></a><span data-ttu-id="42fd2-108">属性</span><span class="sxs-lookup"><span data-stu-id="42fd2-108">Properties</span></span>
|<span data-ttu-id="42fd2-109">属性</span><span class="sxs-lookup"><span data-stu-id="42fd2-109">Property</span></span>|<span data-ttu-id="42fd2-110">类型</span><span class="sxs-lookup"><span data-stu-id="42fd2-110">Type</span></span>|<span data-ttu-id="42fd2-111">说明</span><span class="sxs-lookup"><span data-stu-id="42fd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="42fd2-112">action</span><span class="sxs-lookup"><span data-stu-id="42fd2-112">action</span></span>|[<span data-ttu-id="42fd2-113">configurationManagerActionType</span><span class="sxs-lookup"><span data-stu-id="42fd2-113">configurationManagerActionType</span></span>](../resources/intune-devices-configurationmanageractiontype.md)|<span data-ttu-id="42fd2-114">要在 Configuration Manager 客户端上触发的操作类型。</span><span class="sxs-lookup"><span data-stu-id="42fd2-114">The action type to trigger on Configuration Manager client.</span></span> <span data-ttu-id="42fd2-115">可取值为：`refreshMachinePolicy`、`refreshUserPolicy`、`wakeUpClient`、`appEvaluation`。</span><span class="sxs-lookup"><span data-stu-id="42fd2-115">Possible values are: `refreshMachinePolicy`, `refreshUserPolicy`, `wakeUpClient`, `appEvaluation`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="42fd2-116">关系</span><span class="sxs-lookup"><span data-stu-id="42fd2-116">Relationships</span></span>
<span data-ttu-id="42fd2-117">无</span><span class="sxs-lookup"><span data-stu-id="42fd2-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="42fd2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="42fd2-118">JSON Representation</span></span>
<span data-ttu-id="42fd2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="42fd2-119">Here is a JSON representation of the resource.</span></span>
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



