---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的 Configuration Manager 客户端信息
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1c9e9b88677c925fb33c998af571b23090dcff5
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785054"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="94cfa-103">configurationManagerClientInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="94cfa-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="94cfa-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="94cfa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94cfa-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="94cfa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94cfa-106">从 SCCM 同步的 Configuration Manager 客户端信息</span><span class="sxs-lookup"><span data-stu-id="94cfa-106">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="94cfa-107">属性</span><span class="sxs-lookup"><span data-stu-id="94cfa-107">Properties</span></span>
|<span data-ttu-id="94cfa-108">属性</span><span class="sxs-lookup"><span data-stu-id="94cfa-108">Property</span></span>|<span data-ttu-id="94cfa-109">类型</span><span class="sxs-lookup"><span data-stu-id="94cfa-109">Type</span></span>|<span data-ttu-id="94cfa-110">说明</span><span class="sxs-lookup"><span data-stu-id="94cfa-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94cfa-111">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="94cfa-111">clientIdentifier</span></span>|<span data-ttu-id="94cfa-112">String</span><span class="sxs-lookup"><span data-stu-id="94cfa-112">String</span></span>|<span data-ttu-id="94cfa-113">SCCM 中的 Configuration Manager 客户端 Id</span><span class="sxs-lookup"><span data-stu-id="94cfa-113">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="94cfa-114">isBlocked</span><span class="sxs-lookup"><span data-stu-id="94cfa-114">isBlocked</span></span>|<span data-ttu-id="94cfa-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="94cfa-115">Boolean</span></span>|<span data-ttu-id="94cfa-116">来自 SCCM 的 Configuration Manager 客户端阻止状态</span><span class="sxs-lookup"><span data-stu-id="94cfa-116">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="94cfa-117">关系</span><span class="sxs-lookup"><span data-stu-id="94cfa-117">Relationships</span></span>
<span data-ttu-id="94cfa-118">无</span><span class="sxs-lookup"><span data-stu-id="94cfa-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="94cfa-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94cfa-119">JSON Representation</span></span>
<span data-ttu-id="94cfa-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94cfa-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String",
  "isBlocked": true
}
```



