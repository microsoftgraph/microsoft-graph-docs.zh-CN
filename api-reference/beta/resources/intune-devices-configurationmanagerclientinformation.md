---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的 Configuration Manager 客户端信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 769f6a5172b7a84e9e75a2d7a8f701e195135823
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49231022"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="11ce1-103">configurationManagerClientInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="11ce1-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="11ce1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11ce1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11ce1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11ce1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11ce1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11ce1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11ce1-107">从 SCCM 同步的 Configuration Manager 客户端信息</span><span class="sxs-lookup"><span data-stu-id="11ce1-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="11ce1-108">属性</span><span class="sxs-lookup"><span data-stu-id="11ce1-108">Properties</span></span>
|<span data-ttu-id="11ce1-109">属性</span><span class="sxs-lookup"><span data-stu-id="11ce1-109">Property</span></span>|<span data-ttu-id="11ce1-110">类型</span><span class="sxs-lookup"><span data-stu-id="11ce1-110">Type</span></span>|<span data-ttu-id="11ce1-111">说明</span><span class="sxs-lookup"><span data-stu-id="11ce1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11ce1-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="11ce1-112">clientIdentifier</span></span>|<span data-ttu-id="11ce1-113">String</span><span class="sxs-lookup"><span data-stu-id="11ce1-113">String</span></span>|<span data-ttu-id="11ce1-114">SCCM 中的 Configuration Manager 客户端 Id</span><span class="sxs-lookup"><span data-stu-id="11ce1-114">Configuration Manager Client Id from SCCM</span></span>|
|<span data-ttu-id="11ce1-115">isBlocked</span><span class="sxs-lookup"><span data-stu-id="11ce1-115">isBlocked</span></span>|<span data-ttu-id="11ce1-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="11ce1-116">Boolean</span></span>|<span data-ttu-id="11ce1-117">来自 SCCM 的 Configuration Manager 客户端阻止状态</span><span class="sxs-lookup"><span data-stu-id="11ce1-117">Configuration Manager Client blocked status from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="11ce1-118">关系</span><span class="sxs-lookup"><span data-stu-id="11ce1-118">Relationships</span></span>
<span data-ttu-id="11ce1-119">无</span><span class="sxs-lookup"><span data-stu-id="11ce1-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11ce1-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11ce1-120">JSON Representation</span></span>
<span data-ttu-id="11ce1-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11ce1-121">Here is a JSON representation of the resource.</span></span>
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




