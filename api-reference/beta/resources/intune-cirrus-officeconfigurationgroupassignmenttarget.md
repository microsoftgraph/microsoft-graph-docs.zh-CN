---
title: officeConfigurationGroupAssignmentTarget 资源类型
description: Office 客户端配置 AAD 组分配目标。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a3451d4bddec96c1e21cd605b05cb34d96372ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32526389"
---
# <a name="officeconfigurationgroupassignmenttarget-resource-type"></a><span data-ttu-id="d83e1-103">officeConfigurationGroupAssignmentTarget 资源类型</span><span class="sxs-lookup"><span data-stu-id="d83e1-103">officeConfigurationGroupAssignmentTarget resource type</span></span>

> <span data-ttu-id="d83e1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d83e1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d83e1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d83e1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d83e1-106">Office 客户端配置 AAD 组分配目标。</span><span class="sxs-lookup"><span data-stu-id="d83e1-106">Office client configuration AAD group assignment target.</span></span>

<span data-ttu-id="d83e1-107">继承自[officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span><span class="sxs-lookup"><span data-stu-id="d83e1-107">Inherits from [officeConfigurationAssignmentTarget](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d83e1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d83e1-108">Properties</span></span>
|<span data-ttu-id="d83e1-109">属性</span><span class="sxs-lookup"><span data-stu-id="d83e1-109">Property</span></span>|<span data-ttu-id="d83e1-110">类型</span><span class="sxs-lookup"><span data-stu-id="d83e1-110">Type</span></span>|<span data-ttu-id="d83e1-111">说明</span><span class="sxs-lookup"><span data-stu-id="d83e1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d83e1-112">groupId</span><span class="sxs-lookup"><span data-stu-id="d83e1-112">groupId</span></span>|<span data-ttu-id="d83e1-113">String</span><span class="sxs-lookup"><span data-stu-id="d83e1-113">String</span></span>|<span data-ttu-id="d83e1-114">要将设备配置定向到的 AAD 组的 Id。</span><span class="sxs-lookup"><span data-stu-id="d83e1-114">The Id of the AAD group we are targeting the device configuration to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d83e1-115">关系</span><span class="sxs-lookup"><span data-stu-id="d83e1-115">Relationships</span></span>
<span data-ttu-id="d83e1-116">无</span><span class="sxs-lookup"><span data-stu-id="d83e1-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d83e1-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d83e1-117">JSON Representation</span></span>
<span data-ttu-id="d83e1-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d83e1-118">Here is a JSON representation of the resource.</span></span>
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



