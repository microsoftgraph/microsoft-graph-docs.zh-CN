---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组分配目标。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30153548"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="3ab20-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ab20-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="3ab20-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ab20-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ab20-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ab20-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ab20-106">Office 客户端配置 AAD 组分配目标。</span><span class="sxs-lookup"><span data-stu-id="3ab20-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="3ab20-107">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="3ab20-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="3ab20-108">属性</span><span class="sxs-lookup"><span data-stu-id="3ab20-108">Properties</span></span>
|<span data-ttu-id="3ab20-109">属性</span><span class="sxs-lookup"><span data-stu-id="3ab20-109">Property</span></span>|<span data-ttu-id="3ab20-110">类型</span><span class="sxs-lookup"><span data-stu-id="3ab20-110">Type</span></span>|<span data-ttu-id="3ab20-111">说明</span><span class="sxs-lookup"><span data-stu-id="3ab20-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ab20-112">groupId</span><span class="sxs-lookup"><span data-stu-id="3ab20-112">groupId</span></span>|<span data-ttu-id="3ab20-113">String</span><span class="sxs-lookup"><span data-stu-id="3ab20-113">String</span></span>|<span data-ttu-id="3ab20-114">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="3ab20-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ab20-115">关系</span><span class="sxs-lookup"><span data-stu-id="3ab20-115">Relationships</span></span>
<span data-ttu-id="3ab20-116">无</span><span class="sxs-lookup"><span data-stu-id="3ab20-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ab20-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ab20-117">JSON Representation</span></span>
<span data-ttu-id="3ab20-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ab20-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeConfigurationGroupAssignmentTarget"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeConfigurationGroupAssignmentTarget",
  "groupId": "String"
}
```



