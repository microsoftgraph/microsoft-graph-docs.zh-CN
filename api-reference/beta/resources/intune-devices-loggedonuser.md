---
title: loggedOnUser 资源类型
description: 登录用户
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a2b92d8504ba4854109efa30d0637bca1ea35d7b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522081"
---
# <a name="loggedonuser-resource-type"></a><span data-ttu-id="df4b3-103">loggedOnUser 资源类型</span><span class="sxs-lookup"><span data-stu-id="df4b3-103">loggedOnUser resource type</span></span>

> <span data-ttu-id="df4b3-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="df4b3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="df4b3-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df4b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df4b3-106">登录用户</span><span class="sxs-lookup"><span data-stu-id="df4b3-106">Logged On User</span></span>

## <a name="properties"></a><span data-ttu-id="df4b3-107">属性</span><span class="sxs-lookup"><span data-stu-id="df4b3-107">Properties</span></span>
|<span data-ttu-id="df4b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="df4b3-108">Property</span></span>|<span data-ttu-id="df4b3-109">类型</span><span class="sxs-lookup"><span data-stu-id="df4b3-109">Type</span></span>|<span data-ttu-id="df4b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="df4b3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df4b3-111">userId</span><span class="sxs-lookup"><span data-stu-id="df4b3-111">userId</span></span>|<span data-ttu-id="df4b3-112">String</span><span class="sxs-lookup"><span data-stu-id="df4b3-112">String</span></span>|<span data-ttu-id="df4b3-113">用户 ID</span><span class="sxs-lookup"><span data-stu-id="df4b3-113">User id</span></span>|
|<span data-ttu-id="df4b3-114">lastLogOnDateTime</span><span class="sxs-lookup"><span data-stu-id="df4b3-114">lastLogOnDateTime</span></span>|<span data-ttu-id="df4b3-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df4b3-115">DateTimeOffset</span></span>|<span data-ttu-id="df4b3-116">用户登录的日期时间</span><span class="sxs-lookup"><span data-stu-id="df4b3-116">Date time when user logs on</span></span>|

## <a name="relationships"></a><span data-ttu-id="df4b3-117">关系</span><span class="sxs-lookup"><span data-stu-id="df4b3-117">Relationships</span></span>
<span data-ttu-id="df4b3-118">无</span><span class="sxs-lookup"><span data-stu-id="df4b3-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df4b3-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df4b3-119">JSON Representation</span></span>
<span data-ttu-id="df4b3-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df4b3-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.loggedOnUser"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.loggedOnUser",
  "userId": "String",
  "lastLogOnDateTime": "String (timestamp)"
}
```





