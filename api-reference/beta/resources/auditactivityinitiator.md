---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起方可以是用户、应用程序或系统 (被视为应用程序)
localization_priority: Normal
ms.openlocfilehash: 14c92a4df42c3d8dbcd6836695df8d6caac3cf87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543766"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="7fda3-104">auditActivityInitiator 资源类型</span><span class="sxs-lookup"><span data-stu-id="7fda3-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="7fda3-105">标识启动活动的资源对象。</span><span class="sxs-lookup"><span data-stu-id="7fda3-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="7fda3-106">发起方可以是用户、应用程序或系统 (被视为应用程序)</span><span class="sxs-lookup"><span data-stu-id="7fda3-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="7fda3-107">属性</span><span class="sxs-lookup"><span data-stu-id="7fda3-107">Properties</span></span>
| <span data-ttu-id="7fda3-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fda3-108">Property</span></span>     | <span data-ttu-id="7fda3-109">类型</span><span class="sxs-lookup"><span data-stu-id="7fda3-109">Type</span></span>   |<span data-ttu-id="7fda3-110">说明</span><span class="sxs-lookup"><span data-stu-id="7fda3-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fda3-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="7fda3-111">app</span></span>|[<span data-ttu-id="7fda3-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="7fda3-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="7fda3-113">如果启动活动的资源是一个应用程序, 则此属性指示所有与应用程序相关的信息, 如 appId、Name、servicePrincipalId、Name。</span><span class="sxs-lookup"><span data-stu-id="7fda3-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="7fda3-114">user</span><span class="sxs-lookup"><span data-stu-id="7fda3-114">user</span></span>|[<span data-ttu-id="7fda3-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="7fda3-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="7fda3-116">如果启动活动的资源是用户, 则此属性指示与用户相关的所有信息, 如 userId、Name、UserPrinicpalName。</span><span class="sxs-lookup"><span data-stu-id="7fda3-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7fda3-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fda3-117">JSON representation</span></span>

<span data-ttu-id="7fda3-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fda3-118">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.auditActivityInitiator"
}-->

```json
{
  "app": {"@odata.type": "microsoft.graph.appIdentity"},
  "user": {"@odata.type": "microsoft.graph.userIdentity"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "auditActivityInitiator resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
