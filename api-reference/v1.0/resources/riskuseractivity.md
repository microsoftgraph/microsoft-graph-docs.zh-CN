---
title: riskUserActivity 资源类型
description: riskUserActivity 检测
author: cloudhandler
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 7677832b2887bbb5dcddbeda21481da39f079669
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133222"
---
# <a name="riskuseractivity-resource-type"></a><span data-ttu-id="0f363-103">riskUserActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="0f363-103">riskUserActivity resource type</span></span>

<span data-ttu-id="0f363-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0f363-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0f363-105">表示 Azure AD 用户的风险活动，由 Azure AD Identity Protection 确定。</span><span class="sxs-lookup"><span data-stu-id="0f363-105">Represents the risk activites of an Azure AD user as determined by Azure AD Identity Protection.</span></span>

## <a name="properties"></a><span data-ttu-id="0f363-106">属性</span><span class="sxs-lookup"><span data-stu-id="0f363-106">Properties</span></span>
|<span data-ttu-id="0f363-107">属性</span><span class="sxs-lookup"><span data-stu-id="0f363-107">Property</span></span>|<span data-ttu-id="0f363-108">类型</span><span class="sxs-lookup"><span data-stu-id="0f363-108">Type</span></span>|<span data-ttu-id="0f363-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f363-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f363-110">detail</span><span class="sxs-lookup"><span data-stu-id="0f363-110">detail</span></span>|<span data-ttu-id="0f363-111">riskDetail</span><span class="sxs-lookup"><span data-stu-id="0f363-111">riskDetail</span></span>|<span data-ttu-id="0f363-112">检测到的风险的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0f363-112">Details of the detected risk.</span></span> <span data-ttu-id="0f363-113">可取值为：`none`、`adminGeneratedTemporaryPassword`、`userPerformedSecuredPasswordChange`、`userPerformedSecuredPasswordReset`、`adminConfirmedSigninSafe`、`aiConfirmedSigninSafe`、`userPassedMFADrivenByRiskBasedPolicy`、`adminDismissedAllRiskForUser`、`adminConfirmedSigninCompromised`、`hidden`、`adminConfirmedUserCompromised`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="0f363-113">Possible values are: `none`, `adminGeneratedTemporaryPassword`, `userPerformedSecuredPasswordChange`, `userPerformedSecuredPasswordReset`, `adminConfirmedSigninSafe`, `aiConfirmedSigninSafe`, `userPassedMFADrivenByRiskBasedPolicy`, `adminDismissedAllRiskForUser`, `adminConfirmedSigninCompromised`, `hidden`, `adminConfirmedUserCompromised`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="0f363-114">riskEventTypes</span><span class="sxs-lookup"><span data-stu-id="0f363-114">riskEventTypes</span></span>|<span data-ttu-id="0f363-115">String collection</span><span class="sxs-lookup"><span data-stu-id="0f363-115">String collection</span></span>|<span data-ttu-id="0f363-116">检测到的风险事件的类型。</span><span class="sxs-lookup"><span data-stu-id="0f363-116">The type of risk event detected.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0f363-117">关系</span><span class="sxs-lookup"><span data-stu-id="0f363-117">Relationships</span></span>
<span data-ttu-id="0f363-118">无。</span><span class="sxs-lookup"><span data-stu-id="0f363-118">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0f363-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0f363-119">JSON representation</span></span>
<span data-ttu-id="0f363-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0f363-120">The following is a JSON representation of the resource.</span></span>
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


