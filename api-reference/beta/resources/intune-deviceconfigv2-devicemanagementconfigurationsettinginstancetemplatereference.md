---
title: deviceManagementConfigurationSettingInstanceTemplateReference 资源类型
description: 设置实例模板引用信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d537791337f13ba9fcf3bd19ef77b1c0aec58463
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666833"
---
# <a name="devicemanagementconfigurationsettinginstancetemplatereference-resource-type"></a><span data-ttu-id="bb8f3-103">deviceManagementConfigurationSettingInstanceTemplateReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb8f3-103">deviceManagementConfigurationSettingInstanceTemplateReference resource type</span></span>

<span data-ttu-id="bb8f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb8f3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb8f3-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb8f3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb8f3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb8f3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb8f3-107">设置实例模板引用信息</span><span class="sxs-lookup"><span data-stu-id="bb8f3-107">Setting instance template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="bb8f3-108">属性</span><span class="sxs-lookup"><span data-stu-id="bb8f3-108">Properties</span></span>
|<span data-ttu-id="bb8f3-109">属性</span><span class="sxs-lookup"><span data-stu-id="bb8f3-109">Property</span></span>|<span data-ttu-id="bb8f3-110">类型</span><span class="sxs-lookup"><span data-stu-id="bb8f3-110">Type</span></span>|<span data-ttu-id="bb8f3-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb8f3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb8f3-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="bb8f3-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="bb8f3-113">String</span><span class="sxs-lookup"><span data-stu-id="bb8f3-113">String</span></span>|<span data-ttu-id="bb8f3-114">设置实例模板 ID</span><span class="sxs-lookup"><span data-stu-id="bb8f3-114">Setting instance template id</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb8f3-115">关系</span><span class="sxs-lookup"><span data-stu-id="bb8f3-115">Relationships</span></span>
<span data-ttu-id="bb8f3-116">无</span><span class="sxs-lookup"><span data-stu-id="bb8f3-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb8f3-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb8f3-117">JSON Representation</span></span>
<span data-ttu-id="bb8f3-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb8f3-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplateReference",
  "settingInstanceTemplateId": "String"
}
```




