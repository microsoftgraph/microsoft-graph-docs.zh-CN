---
title: deviceManagementConfigurationDependentOn 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 67e4f4b542fa5d295a7abcd92665325b49349069
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241450"
---
# <a name="devicemanagementconfigurationdependenton-resource-type"></a><span data-ttu-id="ce788-103">deviceManagementConfigurationDependentOn 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce788-103">deviceManagementConfigurationDependentOn resource type</span></span>

<span data-ttu-id="ce788-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ce788-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce788-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ce788-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce788-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ce788-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce788-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ce788-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="ce788-108">属性</span><span class="sxs-lookup"><span data-stu-id="ce788-108">Properties</span></span>
|<span data-ttu-id="ce788-109">属性</span><span class="sxs-lookup"><span data-stu-id="ce788-109">Property</span></span>|<span data-ttu-id="ce788-110">类型</span><span class="sxs-lookup"><span data-stu-id="ce788-110">Type</span></span>|<span data-ttu-id="ce788-111">说明</span><span class="sxs-lookup"><span data-stu-id="ce788-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce788-112">dependentOn</span><span class="sxs-lookup"><span data-stu-id="ce788-112">dependentOn</span></span>|<span data-ttu-id="ce788-113">String</span><span class="sxs-lookup"><span data-stu-id="ce788-113">String</span></span>|<span data-ttu-id="ce788-114">父设置的标识符/父设置选项取决于</span><span class="sxs-lookup"><span data-stu-id="ce788-114">Identifier of parent setting/ parent setting option dependent on</span></span>|
|<span data-ttu-id="ce788-115">parentSettingId</span><span class="sxs-lookup"><span data-stu-id="ce788-115">parentSettingId</span></span>|<span data-ttu-id="ce788-116">String</span><span class="sxs-lookup"><span data-stu-id="ce788-116">String</span></span>|<span data-ttu-id="ce788-117">依赖项的父设置/父设置 id 的标识符</span><span class="sxs-lookup"><span data-stu-id="ce788-117">Identifier of parent setting/ parent setting id dependent on</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce788-118">关系</span><span class="sxs-lookup"><span data-stu-id="ce788-118">Relationships</span></span>
<span data-ttu-id="ce788-119">无</span><span class="sxs-lookup"><span data-stu-id="ce788-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce788-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce788-120">JSON Representation</span></span>
<span data-ttu-id="ce788-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce788-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationDependentOn"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationDependentOn",
  "dependentOn": "String",
  "parentSettingId": "String"
}
```




