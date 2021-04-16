---
title: deviceManagementConfigurationReferenceSettingValue 资源类型
description: ReferenceSettingValue 的模型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1dc92606270cf4c2febcee68905f0c8bd29ced13
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868425"
---
# <a name="devicemanagementconfigurationreferencesettingvalue-resource-type"></a><span data-ttu-id="49ac7-103">deviceManagementConfigurationReferenceSettingValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="49ac7-103">deviceManagementConfigurationReferenceSettingValue resource type</span></span>

<span data-ttu-id="49ac7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49ac7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="49ac7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49ac7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49ac7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49ac7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49ac7-107">ReferenceSettingValue 的模型</span><span class="sxs-lookup"><span data-stu-id="49ac7-107">Model for ReferenceSettingValue</span></span>


<span data-ttu-id="49ac7-108">继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="49ac7-108">Inherits from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>

## <a name="properties"></a><span data-ttu-id="49ac7-109">属性</span><span class="sxs-lookup"><span data-stu-id="49ac7-109">Properties</span></span>
|<span data-ttu-id="49ac7-110">属性</span><span class="sxs-lookup"><span data-stu-id="49ac7-110">Property</span></span>|<span data-ttu-id="49ac7-111">类型</span><span class="sxs-lookup"><span data-stu-id="49ac7-111">Type</span></span>|<span data-ttu-id="49ac7-112">说明</span><span class="sxs-lookup"><span data-stu-id="49ac7-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49ac7-113">值</span><span class="sxs-lookup"><span data-stu-id="49ac7-113">value</span></span>|<span data-ttu-id="49ac7-114">String</span><span class="sxs-lookup"><span data-stu-id="49ac7-114">String</span></span>|<span data-ttu-id="49ac7-115">字符串设置的值。</span><span class="sxs-lookup"><span data-stu-id="49ac7-115">Value of the string setting.</span></span> <span data-ttu-id="49ac7-116">继承自 [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span><span class="sxs-lookup"><span data-stu-id="49ac7-116">Inherited from [deviceManagementConfigurationStringSettingValue](../resources/intune-deviceconfigv2-devicemanagementconfigurationstringsettingvalue.md)</span></span>|
|<span data-ttu-id="49ac7-117">note</span><span class="sxs-lookup"><span data-stu-id="49ac7-117">note</span></span>|<span data-ttu-id="49ac7-118">String</span><span class="sxs-lookup"><span data-stu-id="49ac7-118">String</span></span>|<span data-ttu-id="49ac7-119">管理员可用于放入一些上下文信息的注释</span><span class="sxs-lookup"><span data-stu-id="49ac7-119">A note that admin can use to put some contextual information</span></span>|

## <a name="relationships"></a><span data-ttu-id="49ac7-120">关系</span><span class="sxs-lookup"><span data-stu-id="49ac7-120">Relationships</span></span>
<span data-ttu-id="49ac7-121">无</span><span class="sxs-lookup"><span data-stu-id="49ac7-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49ac7-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49ac7-122">JSON Representation</span></span>
<span data-ttu-id="49ac7-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49ac7-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferenceSettingValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferenceSettingValue",
  "value": "String",
  "note": "String"
}
```




