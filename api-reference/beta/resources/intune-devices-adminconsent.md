---
title: adminConsent 资源类型
description: 管理员同意信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aaac2bb11d90f1e6fec52fae0c17f374c33868ce
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943366"
---
# <a name="adminconsent-resource-type"></a><span data-ttu-id="8e999-103">adminConsent 资源类型</span><span class="sxs-lookup"><span data-stu-id="8e999-103">adminConsent resource type</span></span>

> <span data-ttu-id="8e999-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8e999-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8e999-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8e999-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8e999-106">管理员同意信息。</span><span class="sxs-lookup"><span data-stu-id="8e999-106">Admin consent information.</span></span>

## <a name="properties"></a><span data-ttu-id="8e999-107">属性</span><span class="sxs-lookup"><span data-stu-id="8e999-107">Properties</span></span>
|<span data-ttu-id="8e999-108">属性</span><span class="sxs-lookup"><span data-stu-id="8e999-108">Property</span></span>|<span data-ttu-id="8e999-109">类型</span><span class="sxs-lookup"><span data-stu-id="8e999-109">Type</span></span>|<span data-ttu-id="8e999-110">说明</span><span class="sxs-lookup"><span data-stu-id="8e999-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8e999-111">shareAPNSData</span><span class="sxs-lookup"><span data-stu-id="8e999-111">shareAPNSData</span></span>|[<span data-ttu-id="8e999-112">adminConsentState</span><span class="sxs-lookup"><span data-stu-id="8e999-112">adminConsentState</span></span>](../resources/intune-devices-adminconsentstate.md)|<span data-ttu-id="8e999-113">将用户和设备数据共享到 Apple 的管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="8e999-113">The admin consent state of sharing user and device data to Apple.</span></span> <span data-ttu-id="8e999-114">可取值为：`notConfigured`、`granted`、`notGranted`。</span><span class="sxs-lookup"><span data-stu-id="8e999-114">Possible values are: `notConfigured`, `granted`, `notGranted`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8e999-115">关系</span><span class="sxs-lookup"><span data-stu-id="8e999-115">Relationships</span></span>
<span data-ttu-id="8e999-116">无</span><span class="sxs-lookup"><span data-stu-id="8e999-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8e999-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8e999-117">JSON Representation</span></span>
<span data-ttu-id="8e999-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8e999-118">Here is a JSON representation of the resource.</span></span>
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




