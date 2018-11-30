---
title: windowsKioskActiveDirectoryGroup 资源类型
description: 用于标识为网亭配置 Azure Directory 组的类
ms.openlocfilehash: 18e876b50bdc8c8946bd511348d6ed3a6fc8fe5c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043257"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="c9f86-103">windowsKioskActiveDirectoryGroup 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9f86-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="c9f86-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c9f86-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c9f86-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c9f86-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9f86-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c9f86-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c9f86-107">用于标识为网亭配置 Azure Directory 组的类</span><span class="sxs-lookup"><span data-stu-id="c9f86-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>

<span data-ttu-id="c9f86-108">继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="c9f86-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c9f86-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9f86-109">Properties</span></span>
|<span data-ttu-id="c9f86-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9f86-110">Property</span></span>|<span data-ttu-id="c9f86-111">类型</span><span class="sxs-lookup"><span data-stu-id="c9f86-111">Type</span></span>|<span data-ttu-id="c9f86-112">说明</span><span class="sxs-lookup"><span data-stu-id="c9f86-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9f86-113">groupName</span><span class="sxs-lookup"><span data-stu-id="c9f86-113">groupName</span></span>|<span data-ttu-id="c9f86-114">字符串</span><span class="sxs-lookup"><span data-stu-id="c9f86-114">String</span></span>|<span data-ttu-id="c9f86-115">将锁定到此网亭配置 AD 组的名称</span><span class="sxs-lookup"><span data-stu-id="c9f86-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9f86-116">Relationships</span><span class="sxs-lookup"><span data-stu-id="c9f86-116">Relationships</span></span>
<span data-ttu-id="c9f86-117">无</span><span class="sxs-lookup"><span data-stu-id="c9f86-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c9f86-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9f86-118">JSON Representation</span></span>
<span data-ttu-id="c9f86-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9f86-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





