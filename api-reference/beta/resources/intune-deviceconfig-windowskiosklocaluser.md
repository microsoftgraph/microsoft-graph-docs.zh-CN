---
title: windowsKioskLocalUser 资源类型
description: 用于标识网亭配置的本地帐户的类
ms.openlocfilehash: 1b5b8837f4f93005dabf839a7fc20e3b05b1fbf9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043058"
---
# <a name="windowskiosklocaluser-resource-type"></a><span data-ttu-id="85bec-103">windowsKioskLocalUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="85bec-103">windowsKioskLocalUser resource type</span></span>

> <span data-ttu-id="85bec-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="85bec-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="85bec-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="85bec-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="85bec-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="85bec-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="85bec-107">用于标识网亭配置的本地帐户的类</span><span class="sxs-lookup"><span data-stu-id="85bec-107">The class used to identify a local account for the kiosk configuration</span></span>

<span data-ttu-id="85bec-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="85bec-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="85bec-109">属性</span><span class="sxs-lookup"><span data-stu-id="85bec-109">Properties</span></span>
|<span data-ttu-id="85bec-110">属性</span><span class="sxs-lookup"><span data-stu-id="85bec-110">Property</span></span>|<span data-ttu-id="85bec-111">类型</span><span class="sxs-lookup"><span data-stu-id="85bec-111">Type</span></span>|<span data-ttu-id="85bec-112">说明</span><span class="sxs-lookup"><span data-stu-id="85bec-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85bec-113">userName</span><span class="sxs-lookup"><span data-stu-id="85bec-113">userName</span></span>|<span data-ttu-id="85bec-114">String</span><span class="sxs-lookup"><span data-stu-id="85bec-114">String</span></span>|<span data-ttu-id="85bec-115">将锁定到此网亭配置本地用户</span><span class="sxs-lookup"><span data-stu-id="85bec-115">The local user that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="85bec-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="85bec-116">Relationships</span></span>
<span data-ttu-id="85bec-117">无</span><span class="sxs-lookup"><span data-stu-id="85bec-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="85bec-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85bec-118">JSON Representation</span></span>
<span data-ttu-id="85bec-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85bec-119">Here is a JSON representation of the resource.</span></span>
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





