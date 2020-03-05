---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的 Configuration Manager 客户端信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67c1a4b4a9ac570b4acd71a1ce819f9705fd32e3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528672"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="45cab-103">configurationManagerClientInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="45cab-103">configurationManagerClientInformation resource type</span></span>

<span data-ttu-id="45cab-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="45cab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45cab-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="45cab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45cab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="45cab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45cab-107">从 SCCM 同步的 Configuration Manager 客户端信息</span><span class="sxs-lookup"><span data-stu-id="45cab-107">Configuration Manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="45cab-108">属性</span><span class="sxs-lookup"><span data-stu-id="45cab-108">Properties</span></span>
|<span data-ttu-id="45cab-109">属性</span><span class="sxs-lookup"><span data-stu-id="45cab-109">Property</span></span>|<span data-ttu-id="45cab-110">类型</span><span class="sxs-lookup"><span data-stu-id="45cab-110">Type</span></span>|<span data-ttu-id="45cab-111">说明</span><span class="sxs-lookup"><span data-stu-id="45cab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45cab-112">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="45cab-112">clientIdentifier</span></span>|<span data-ttu-id="45cab-113">String</span><span class="sxs-lookup"><span data-stu-id="45cab-113">String</span></span>|<span data-ttu-id="45cab-114">SCCM 中的 Configuration Manager 客户端 Id</span><span class="sxs-lookup"><span data-stu-id="45cab-114">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="45cab-115">关系</span><span class="sxs-lookup"><span data-stu-id="45cab-115">Relationships</span></span>
<span data-ttu-id="45cab-116">无</span><span class="sxs-lookup"><span data-stu-id="45cab-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="45cab-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45cab-117">JSON Representation</span></span>
<span data-ttu-id="45cab-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45cab-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.configurationManagerClientInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.configurationManagerClientInformation",
  "clientIdentifier": "String"
}
```



