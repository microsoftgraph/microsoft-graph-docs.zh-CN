---
title: deviceManagementConfigurationSettingDependedOnBy 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f3d9b6bde7217460867ab7e9b77853fcb366e38c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49241268"
---
# <a name="devicemanagementconfigurationsettingdependedonby-resource-type"></a><span data-ttu-id="20f59-103">deviceManagementConfigurationSettingDependedOnBy 资源类型</span><span class="sxs-lookup"><span data-stu-id="20f59-103">deviceManagementConfigurationSettingDependedOnBy resource type</span></span>

<span data-ttu-id="20f59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20f59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20f59-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20f59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20f59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20f59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20f59-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20f59-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20f59-108">属性</span><span class="sxs-lookup"><span data-stu-id="20f59-108">Properties</span></span>
|<span data-ttu-id="20f59-109">属性</span><span class="sxs-lookup"><span data-stu-id="20f59-109">Property</span></span>|<span data-ttu-id="20f59-110">类型</span><span class="sxs-lookup"><span data-stu-id="20f59-110">Type</span></span>|<span data-ttu-id="20f59-111">说明</span><span class="sxs-lookup"><span data-stu-id="20f59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f59-112">dependedOnBy</span><span class="sxs-lookup"><span data-stu-id="20f59-112">dependedOnBy</span></span>|<span data-ttu-id="20f59-113">String</span><span class="sxs-lookup"><span data-stu-id="20f59-113">String</span></span>|<span data-ttu-id="20f59-114">依赖于当前设置的子设置的标识符</span><span class="sxs-lookup"><span data-stu-id="20f59-114">Identifier of child setting that is dependent on the current setting</span></span>|
|<span data-ttu-id="20f59-115">必需</span><span class="sxs-lookup"><span data-stu-id="20f59-115">required</span></span>|<span data-ttu-id="20f59-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="20f59-116">Boolean</span></span>|<span data-ttu-id="20f59-117">根据父设置的选择确定是否需要子设置的值</span><span class="sxs-lookup"><span data-stu-id="20f59-117">Value that determines if the child setting is required based on the parent setting's selection</span></span>|

## <a name="relationships"></a><span data-ttu-id="20f59-118">关系</span><span class="sxs-lookup"><span data-stu-id="20f59-118">Relationships</span></span>
<span data-ttu-id="20f59-119">无</span><span class="sxs-lookup"><span data-stu-id="20f59-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20f59-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20f59-120">JSON Representation</span></span>
<span data-ttu-id="20f59-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20f59-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingDependedOnBy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingDependedOnBy",
  "dependedOnBy": "String",
  "required": true
}
```




