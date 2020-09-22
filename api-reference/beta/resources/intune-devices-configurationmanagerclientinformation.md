---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的 Configuration Manager 客户端信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 22844c063bb119d956740045c088be4fad59f89d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060634"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="09594-103">configurationManagerClientInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="09594-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="09594-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="09594-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="09594-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="09594-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="09594-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09594-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09594-107">从 SCCM 同步的 Configuration Manager 客户端信息</span><span class="sxs-lookup"><span data-stu-id="09594-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="09594-108">属性</span><span class="sxs-lookup"><span data-stu-id="09594-108">Properties</span></span>
|<span data-ttu-id="09594-109">属性</span><span class="sxs-lookup"><span data-stu-id="09594-109">Property</span></span>|<span data-ttu-id="09594-110">类型</span><span class="sxs-lookup"><span data-stu-id="09594-110">Type</span></span>|<span data-ttu-id="09594-111">说明</span><span class="sxs-lookup"><span data-stu-id="09594-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09594-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="09594-112">clientIdentifier</span></span>|<span data-ttu-id="09594-113">String</span><span class="sxs-lookup"><span data-stu-id="09594-113">String</span></span>|<span data-ttu-id="09594-114">SCCM 中的 Configuration Manager 客户端 Id</span><span class="sxs-lookup"><span data-stu-id="09594-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="09594-115">isBlocked</span><span class="sxs-lookup"><span data-stu-id="09594-115">isBlocked</span></span>|<span data-ttu-id="09594-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="09594-116">Boolean</span></span>|<span data-ttu-id="09594-117">来自 SCCM 的 Configuration Manager 客户端阻止状态</span><span class="sxs-lookup"><span data-stu-id="09594-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="09594-118">关系</span><span class="sxs-lookup"><span data-stu-id="09594-118">Relationships</span></span>
<span data-ttu-id="09594-119">无</span><span class="sxs-lookup"><span data-stu-id="09594-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="09594-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="09594-120">JSON Representation</span></span>
<span data-ttu-id="09594-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09594-121">Here is a JSON representation of the resource.</span></span>
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






