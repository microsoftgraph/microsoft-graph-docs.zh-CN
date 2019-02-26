---
title: adminConsent 资源类型
description: 管理员同意信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8f46e379a47bd7b08be1427115c785452543dfbf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157937"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="d7b3a-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="d7b3a-103">adminConsent resource type</span></span>

> <span data-ttu-id="d7b3a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d7b3a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d7b3a-106">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="d7b3a-107">属性</span><span class="sxs-lookup"><span data-stu-id="d7b3a-107">Properties</span></span>
|<span data-ttu-id="d7b3a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d7b3a-108">Property</span></span>|<span data-ttu-id="d7b3a-109">类型</span><span class="sxs-lookup"><span data-stu-id="d7b3a-109">Type</span></span>|<span data-ttu-id="d7b3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="d7b3a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d7b3a-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="d7b3a-111">shareAPNSData</span></span>|[<span data-ttu-id="d7b3a-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="d7b3a-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="d7b3a-113">将用户和设备数据共享到 Apple 的管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="d7b3a-114">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7b3a-115">Relationships</span><span class="sxs-lookup"><span data-stu-id="d7b3a-115">Relationships</span></span>
<span data-ttu-id="d7b3a-116">无</span><span class="sxs-lookup"><span data-stu-id="d7b3a-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d7b3a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d7b3a-117">JSON Representation</span></span>
<span data-ttu-id="d7b3a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d7b3a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.adminConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsent",
  "shareAPNSData": "String"
}
```




