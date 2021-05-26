---
title: deviceManagementConfigurationSettingInstance 资源类型
description: 在策略中设置实例
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 84b3b3a641fc8710bdd1b4266f15436084d01bdc
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665600"
---
# <a name="devicemanagementconfigurationsettinginstance-resource-type"></a><span data-ttu-id="7887e-103">deviceManagementConfigurationSettingInstance 资源类型</span><span class="sxs-lookup"><span data-stu-id="7887e-103">deviceManagementConfigurationSettingInstance resource type</span></span>

<span data-ttu-id="7887e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7887e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7887e-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7887e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7887e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7887e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7887e-107">在策略中设置实例</span><span class="sxs-lookup"><span data-stu-id="7887e-107">Setting instance within policy</span></span>

## <a name="properties"></a><span data-ttu-id="7887e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7887e-108">Properties</span></span>
|<span data-ttu-id="7887e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7887e-109">Property</span></span>|<span data-ttu-id="7887e-110">类型</span><span class="sxs-lookup"><span data-stu-id="7887e-110">Type</span></span>|<span data-ttu-id="7887e-111">说明</span><span class="sxs-lookup"><span data-stu-id="7887e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7887e-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="7887e-112">settingDefinitionId</span></span>|<span data-ttu-id="7887e-113">String</span><span class="sxs-lookup"><span data-stu-id="7887e-113">String</span></span>|<span data-ttu-id="7887e-114">设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="7887e-114">Setting Definition Id</span></span>|
|<span data-ttu-id="7887e-115">settingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="7887e-115">settingInstanceTemplateReference</span></span>|[<span data-ttu-id="7887e-116">deviceManagementConfigurationSettingInstanceTemplateReference</span><span class="sxs-lookup"><span data-stu-id="7887e-116">deviceManagementConfigurationSettingInstanceTemplateReference</span></span>](../resources/intune-deviceconfigv2-devicemanagementconfigurationsettinginstancetemplatereference.md)|<span data-ttu-id="7887e-117">设置实例模板引用</span><span class="sxs-lookup"><span data-stu-id="7887e-117">Setting Instance Template Reference</span></span>|

## <a name="relationships"></a><span data-ttu-id="7887e-118">关系</span><span class="sxs-lookup"><span data-stu-id="7887e-118">Relationships</span></span>
<span data-ttu-id="7887e-119">无</span><span class="sxs-lookup"><span data-stu-id="7887e-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7887e-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7887e-120">JSON Representation</span></span>
<span data-ttu-id="7887e-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7887e-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstance",
  "settingDefinitionId": "String",
  "settingInstanceTemplateReference": {
    "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
    "settingInstanceTemplateId": "String"
  }
}
```




