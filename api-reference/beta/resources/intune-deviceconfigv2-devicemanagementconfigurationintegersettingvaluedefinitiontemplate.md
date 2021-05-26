---
title: deviceManagementConfigurationIntegerSettingValueDefinitionTemplate 资源类型
description: 整数设置值定义模板
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 488c71fd7f242604a2bcd8bbdcc2ca7f526bd4d7
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666843"
---
# <a name="devicemanagementconfigurationintegersettingvaluedefinitiontemplate-resource-type"></a><span data-ttu-id="51a29-103">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate 资源类型</span><span class="sxs-lookup"><span data-stu-id="51a29-103">deviceManagementConfigurationIntegerSettingValueDefinitionTemplate resource type</span></span>

<span data-ttu-id="51a29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51a29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51a29-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="51a29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51a29-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51a29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51a29-107">整数设置值定义模板</span><span class="sxs-lookup"><span data-stu-id="51a29-107">Integer Setting Value Definition Template</span></span>

## <a name="properties"></a><span data-ttu-id="51a29-108">属性</span><span class="sxs-lookup"><span data-stu-id="51a29-108">Properties</span></span>
|<span data-ttu-id="51a29-109">属性</span><span class="sxs-lookup"><span data-stu-id="51a29-109">Property</span></span>|<span data-ttu-id="51a29-110">类型</span><span class="sxs-lookup"><span data-stu-id="51a29-110">Type</span></span>|<span data-ttu-id="51a29-111">说明</span><span class="sxs-lookup"><span data-stu-id="51a29-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51a29-112">minValue</span><span class="sxs-lookup"><span data-stu-id="51a29-112">minValue</span></span>|<span data-ttu-id="51a29-113">Int32</span><span class="sxs-lookup"><span data-stu-id="51a29-113">Int32</span></span>|<span data-ttu-id="51a29-114">整数设置最小值。</span><span class="sxs-lookup"><span data-stu-id="51a29-114">Integer Setting Minimum Value.</span></span> <span data-ttu-id="51a29-115">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="51a29-115">Valid values -2147483648 to 2147483647</span></span>|
|<span data-ttu-id="51a29-116">maxValue</span><span class="sxs-lookup"><span data-stu-id="51a29-116">maxValue</span></span>|<span data-ttu-id="51a29-117">Int32</span><span class="sxs-lookup"><span data-stu-id="51a29-117">Int32</span></span>|<span data-ttu-id="51a29-118">整数设置最大值。</span><span class="sxs-lookup"><span data-stu-id="51a29-118">Integer Setting Maximum Value.</span></span> <span data-ttu-id="51a29-119">有效值 -2147483648 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="51a29-119">Valid values -2147483648 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="51a29-120">关系</span><span class="sxs-lookup"><span data-stu-id="51a29-120">Relationships</span></span>
<span data-ttu-id="51a29-121">无</span><span class="sxs-lookup"><span data-stu-id="51a29-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="51a29-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="51a29-122">JSON Representation</span></span>
<span data-ttu-id="51a29-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51a29-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationIntegerSettingValueDefinitionTemplate",
  "minValue": 1024,
  "maxValue": 1024
}
```




