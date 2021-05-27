---
title: registrationEnforcement 资源类型
description: 在登录时强制注册。
author: mjsantani
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 86d3e974ccfebdf0011c9c19f881096e3fb2ba40
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682870"
---
# <a name="registrationenforcement-resource-type"></a><span data-ttu-id="f9079-103">registrationEnforcement 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9079-103">registrationEnforcement resource type</span></span>

<span data-ttu-id="f9079-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9079-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9079-105">在登录时强制注册。</span><span class="sxs-lookup"><span data-stu-id="f9079-105">Enforce registration at sign-in time.</span></span> <span data-ttu-id="f9079-106">目前，这仅用于提醒用户使用"authenticationMethodsRegistrationCampaign" (Microsoft Authenticator) 设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f9079-106">This can currently only be used to remind users to set up targeted authentication methods (Microsoft Authenticator) using the 'authenticationMethodsRegistrationCampaign\`.</span></span>

## <a name="properties"></a><span data-ttu-id="f9079-107">属性</span><span class="sxs-lookup"><span data-stu-id="f9079-107">Properties</span></span>
|<span data-ttu-id="f9079-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9079-108">Property</span></span>|<span data-ttu-id="f9079-109">类型</span><span class="sxs-lookup"><span data-stu-id="f9079-109">Type</span></span>|<span data-ttu-id="f9079-110">说明</span><span class="sxs-lookup"><span data-stu-id="f9079-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9079-111">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="f9079-111">authenticationMethodsRegistrationCampaign</span></span>|[<span data-ttu-id="f9079-112">authenticationMethodsRegistrationCampaign</span><span class="sxs-lookup"><span data-stu-id="f9079-112">authenticationMethodsRegistrationCampaign</span></span>](../resources/authenticationmethodsregistrationcampaign.md)|<span data-ttu-id="f9079-113">开展市场活动以提醒用户设置目标身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="f9079-113">Run campaigns to remind users to setup targeted authentication methods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9079-114">关系</span><span class="sxs-lookup"><span data-stu-id="f9079-114">Relationships</span></span>
<span data-ttu-id="f9079-115">无。</span><span class="sxs-lookup"><span data-stu-id="f9079-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f9079-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9079-116">JSON representation</span></span>
<span data-ttu-id="f9079-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9079-117">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.registrationEnforcement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.registrationEnforcement",
  "authenticationMethodsRegistrationCampaign": {
    "@odata.type": "microsoft.graph.authenticationMethodsRegistrationCampaign"
  }
}
```
