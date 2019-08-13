---
title: configurationManagerClientInformation 资源类型
description: 从 SCCM 同步的 Configuration manager 客户端信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ae7d36b353b989d4256294872fba4c4f225d2668
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371476"
---
# <a name="configurationmanagerclientinformation-resource-type"></a><span data-ttu-id="bf63a-103">configurationManagerClientInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf63a-103">configurationManagerClientInformation resource type</span></span>

> <span data-ttu-id="bf63a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bf63a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf63a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bf63a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf63a-106">从 SCCM 同步的 Configuration manager 客户端信息</span><span class="sxs-lookup"><span data-stu-id="bf63a-106">Configuration manager client information synced from SCCM</span></span>

## <a name="properties"></a><span data-ttu-id="bf63a-107">属性</span><span class="sxs-lookup"><span data-stu-id="bf63a-107">Properties</span></span>
|<span data-ttu-id="bf63a-108">属性</span><span class="sxs-lookup"><span data-stu-id="bf63a-108">Property</span></span>|<span data-ttu-id="bf63a-109">类型</span><span class="sxs-lookup"><span data-stu-id="bf63a-109">Type</span></span>|<span data-ttu-id="bf63a-110">说明</span><span class="sxs-lookup"><span data-stu-id="bf63a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf63a-111">clientIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf63a-111">clientIdentifier</span></span>|<span data-ttu-id="bf63a-112">String</span><span class="sxs-lookup"><span data-stu-id="bf63a-112">String</span></span>|<span data-ttu-id="bf63a-113">SCCM 中的 Configuration Manager 客户端 Id</span><span class="sxs-lookup"><span data-stu-id="bf63a-113">Configuration Manager Client Id from SCCM</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf63a-114">关系</span><span class="sxs-lookup"><span data-stu-id="bf63a-114">Relationships</span></span>
<span data-ttu-id="bf63a-115">无</span><span class="sxs-lookup"><span data-stu-id="bf63a-115">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf63a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf63a-116">JSON Representation</span></span>
<span data-ttu-id="bf63a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf63a-117">Here is a JSON representation of the resource.</span></span>
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



