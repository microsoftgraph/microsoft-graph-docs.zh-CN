---
title: windowsKioskLocalUser 资源类型
description: 用于标识展台配置的本地帐户的类
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1c375de52d9fc294a308eb7c5b2652ef13db0c4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548080"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="f786f-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="f786f-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="f786f-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f786f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f786f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f786f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f786f-106">用于标识展台配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="f786f-106">The class used to identify a local account for the kiosk configuration</span></span>


<span data-ttu-id="f786f-107">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="f786f-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f786f-108">属性</span><span class="sxs-lookup"><span data-stu-id="f786f-108">Properties</span></span>
|<span data-ttu-id="f786f-109">属性</span><span class="sxs-lookup"><span data-stu-id="f786f-109">Property</span></span>|<span data-ttu-id="f786f-110">类型</span><span class="sxs-lookup"><span data-stu-id="f786f-110">Type</span></span>|<span data-ttu-id="f786f-111">说明</span><span class="sxs-lookup"><span data-stu-id="f786f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f786f-112">userName</span><span class="sxs-lookup"><span data-stu-id="f786f-112">userName</span></span>|<span data-ttu-id="f786f-113">String</span><span class="sxs-lookup"><span data-stu-id="f786f-113">String</span></span>|<span data-ttu-id="f786f-114">将锁定到此展台配置的本地用户</span><span class="sxs-lookup"><span data-stu-id="f786f-114">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="f786f-115">关系</span><span class="sxs-lookup"><span data-stu-id="f786f-115">Relationships</span></span>
<span data-ttu-id="f786f-116">无</span><span class="sxs-lookup"><span data-stu-id="f786f-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f786f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f786f-117">JSON Representation</span></span>
<span data-ttu-id="f786f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f786f-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskLocalUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskLocalUser",
  "userName": "String"
}
```





