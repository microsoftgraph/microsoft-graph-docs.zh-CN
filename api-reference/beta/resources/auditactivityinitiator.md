---
title: auditActivityInitiator 资源类型
description: 标识启动活动的资源对象。 发起人可以是用户、 应用程序或系统 （它被认为是作为应用程序）
ms.openlocfilehash: 834b39f67a9a3a251c61f15d3b1fa8aa964870e9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046199"
---
# <a name="auditactivityinitiator-resource-type"></a><span data-ttu-id="34495-104">auditActivityInitiator 资源类型</span><span class="sxs-lookup"><span data-stu-id="34495-104">auditActivityInitiator resource type</span></span>
<span data-ttu-id="34495-105">标识启动活动的资源对象。</span><span class="sxs-lookup"><span data-stu-id="34495-105">Identity the resource object that initiates the activity.</span></span> <span data-ttu-id="34495-106">发起人可以是用户、 应用程序或系统 （它被认为是作为应用程序）</span><span class="sxs-lookup"><span data-stu-id="34495-106">The initiator can be a user, an app or a system (which is considered as an app)</span></span>



## <a name="properties"></a><span data-ttu-id="34495-107">属性</span><span class="sxs-lookup"><span data-stu-id="34495-107">Properties</span></span>
| <span data-ttu-id="34495-108">属性</span><span class="sxs-lookup"><span data-stu-id="34495-108">Property</span></span>     | <span data-ttu-id="34495-109">类型</span><span class="sxs-lookup"><span data-stu-id="34495-109">Type</span></span>   |<span data-ttu-id="34495-110">说明</span><span class="sxs-lookup"><span data-stu-id="34495-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34495-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="34495-111">app</span></span>|[<span data-ttu-id="34495-112">appIdentity</span><span class="sxs-lookup"><span data-stu-id="34495-112">appIdentity</span></span>](appidentity.md)|<span data-ttu-id="34495-113">如果启动活动资源是应用程序，此属性指示所有应用程序相关信息，appId，如姓名、 servicePrincipalId，名称。</span><span class="sxs-lookup"><span data-stu-id="34495-113">If the resource initiating the activity is an app, this property indicates all the app related information like appId, Name, servicePrincipalId, Name.</span></span>|
|<span data-ttu-id="34495-114">user</span><span class="sxs-lookup"><span data-stu-id="34495-114">user</span></span>|[<span data-ttu-id="34495-115">userIdentity</span><span class="sxs-lookup"><span data-stu-id="34495-115">userIdentity</span></span>](useridentity.md)|<span data-ttu-id="34495-116">如果启动了此活动的资源是用户，此属性指示所有用户相关的用户 Id，名称、 UserPrinicpalName 类似的信息。</span><span class="sxs-lookup"><span data-stu-id="34495-116">If the resource initiating the activity is a user, this property Indicates all the user related information like userId, Name, UserPrinicpalName.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="34495-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="34495-117">JSON representation</span></span>

<span data-ttu-id="34495-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34495-118">Here is a JSON representation of the resource.</span></span>

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