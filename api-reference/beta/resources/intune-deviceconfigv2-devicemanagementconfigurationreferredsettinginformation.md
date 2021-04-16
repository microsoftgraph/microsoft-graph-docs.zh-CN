---
title: deviceManagementConfigurationReferredSettingInformation 资源类型
description: 有关可重用设置的参考设置信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 12003df5ec19bdf32b213945033eb9d5e73b9692
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868391"
---
# <a name="devicemanagementconfigurationreferredsettinginformation-resource-type"></a><span data-ttu-id="6b1b7-103">deviceManagementConfigurationReferredSettingInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b1b7-103">deviceManagementConfigurationReferredSettingInformation resource type</span></span>

<span data-ttu-id="6b1b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b1b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6b1b7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b1b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b1b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b1b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b1b7-107">有关可重用设置的参考设置信息</span><span class="sxs-lookup"><span data-stu-id="6b1b7-107">Referred setting information about reusable setting</span></span>

## <a name="properties"></a><span data-ttu-id="6b1b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b1b7-108">Properties</span></span>
|<span data-ttu-id="6b1b7-109">属性</span><span class="sxs-lookup"><span data-stu-id="6b1b7-109">Property</span></span>|<span data-ttu-id="6b1b7-110">类型</span><span class="sxs-lookup"><span data-stu-id="6b1b7-110">Type</span></span>|<span data-ttu-id="6b1b7-111">说明</span><span class="sxs-lookup"><span data-stu-id="6b1b7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b1b7-112">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="6b1b7-112">settingDefinitionId</span></span>|<span data-ttu-id="6b1b7-113">String</span><span class="sxs-lookup"><span data-stu-id="6b1b7-113">String</span></span>|<span data-ttu-id="6b1b7-114">设置引用到设置的定义 ID。</span><span class="sxs-lookup"><span data-stu-id="6b1b7-114">Setting definition id that is being referred to a setting.</span></span> <span data-ttu-id="6b1b7-115">适用于可重用设置</span><span class="sxs-lookup"><span data-stu-id="6b1b7-115">Applicable for reusable setting</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b1b7-116">关系</span><span class="sxs-lookup"><span data-stu-id="6b1b7-116">Relationships</span></span>
<span data-ttu-id="6b1b7-117">无</span><span class="sxs-lookup"><span data-stu-id="6b1b7-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b1b7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b1b7-118">JSON Representation</span></span>
<span data-ttu-id="6b1b7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b1b7-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationReferredSettingInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationReferredSettingInformation",
  "settingDefinitionId": "String"
}
```




