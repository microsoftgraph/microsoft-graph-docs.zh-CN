---
title: riskUserActivity 资源类型
description: riskUserActivity 检测
author: cloudhandler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b2b20a5796f5e1266271cd29d0768aa52927062a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991871"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="efe53-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="efe53-103">riskUserActivity resource type</span></span>

<span data-ttu-id="efe53-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="efe53-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="efe53-105">表示 azure AD 用户的风险活动，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="efe53-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="efe53-106">属性</span><span class="sxs-lookup"><span data-stu-id="efe53-106">Properties</span></span>
|<span data-ttu-id="efe53-107">属性</span><span class="sxs-lookup"><span data-stu-id="efe53-107">Property</span></span>|<span data-ttu-id="efe53-108">类型</span><span class="sxs-lookup"><span data-stu-id="efe53-108">Type</span></span>|<span data-ttu-id="efe53-109">说明</span><span class="sxs-lookup"><span data-stu-id="efe53-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="efe53-110">介绍</span><span class="sxs-lookup"><span data-stu-id="efe53-110">detail</span></span>|<span data-ttu-id="efe53-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="efe53-111">riskDetail</span></span>|<span data-ttu-id="efe53-112">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="efe53-112">Details of the detected risk.</span></span> <span data-ttu-id="efe53-113">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="efe53-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="efe53-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="efe53-114">riskEventTypes</span></span>|<span data-ttu-id="efe53-115">String collection</span><span class="sxs-lookup"><span data-stu-id="efe53-115">String collection</span></span>|<span data-ttu-id="efe53-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="efe53-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="efe53-117">关系</span><span class="sxs-lookup"><span data-stu-id="efe53-117">Relationships</span></span>
<span data-ttu-id="efe53-118">无。</span><span class="sxs-lookup"><span data-stu-id="efe53-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="efe53-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="efe53-119">JSON representation</span></span>
<span data-ttu-id="efe53-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="efe53-120">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.riskUserActivity"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.riskUserActivity",
  "riskEventTypes": [
    "String"
  ],
  "detail": "String"
}
```


