---
title: unaryManagementConditionExpression 资源类型
description: 使用一元运算计算的管理条件表达式。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: dcede3b729f22c7bf12342285bfc2cbf654e2068
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298839"
---
# <a name="unarymanagementconditionexpression-resource-type"></a><span data-ttu-id="5403a-103">unaryManagementConditionExpression 资源类型</span><span class="sxs-lookup"><span data-stu-id="5403a-103">unaryManagementConditionExpression resource type</span></span>

<span data-ttu-id="5403a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5403a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5403a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5403a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5403a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5403a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5403a-107">使用一元运算计算的管理条件表达式。</span><span class="sxs-lookup"><span data-stu-id="5403a-107">A management condition expression that is evaluated using a unary operation.</span></span>


<span data-ttu-id="5403a-108">继承自 [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span><span class="sxs-lookup"><span data-stu-id="5403a-108">Inherits from [managementConditionExpressionModel](../resources/intune-fencing-managementconditionexpressionmodel.md)</span></span>

## <a name="properties"></a><span data-ttu-id="5403a-109">属性</span><span class="sxs-lookup"><span data-stu-id="5403a-109">Properties</span></span>
|<span data-ttu-id="5403a-110">属性</span><span class="sxs-lookup"><span data-stu-id="5403a-110">Property</span></span>|<span data-ttu-id="5403a-111">类型</span><span class="sxs-lookup"><span data-stu-id="5403a-111">Type</span></span>|<span data-ttu-id="5403a-112">Description</span><span class="sxs-lookup"><span data-stu-id="5403a-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5403a-113">operator</span><span class="sxs-lookup"><span data-stu-id="5403a-113">operator</span></span>|[<span data-ttu-id="5403a-114">unaryManagementConditionExpressionOperatorType</span><span class="sxs-lookup"><span data-stu-id="5403a-114">unaryManagementConditionExpressionOperatorType</span></span>](../resources/intune-fencing-unarymanagementconditionexpressionoperatortype.md)|<span data-ttu-id="5403a-115">在一元运算的计算中使用的运算符。</span><span class="sxs-lookup"><span data-stu-id="5403a-115">The operator used in the evaluation of the unary operation.</span></span> <span data-ttu-id="5403a-116">可能的值是： `not` 。</span><span class="sxs-lookup"><span data-stu-id="5403a-116">Possible values are: `not`.</span></span>|
|<span data-ttu-id="5403a-117">运算符</span><span class="sxs-lookup"><span data-stu-id="5403a-117">operand</span></span>|[<span data-ttu-id="5403a-118">managementConditionExpressionModel</span><span class="sxs-lookup"><span data-stu-id="5403a-118">managementConditionExpressionModel</span></span>](../resources/intune-fencing-managementconditionexpressionmodel.md)|<span data-ttu-id="5403a-119">一元运算的操作数。</span><span class="sxs-lookup"><span data-stu-id="5403a-119">The operand of the unary operation.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5403a-120">关系</span><span class="sxs-lookup"><span data-stu-id="5403a-120">Relationships</span></span>
<span data-ttu-id="5403a-121">无</span><span class="sxs-lookup"><span data-stu-id="5403a-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5403a-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5403a-122">JSON Representation</span></span>
<span data-ttu-id="5403a-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5403a-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unaryManagementConditionExpression"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unaryManagementConditionExpression",
  "operator": "String",
  "operand": {
    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
    "operator": "String",
    "firstOperand": {
      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
      "operator": "String",
      "firstOperand": {
        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
        "operator": "String",
        "firstOperand": {
          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
          "operator": "String",
          "firstOperand": {
            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
            "operator": "String",
            "firstOperand": {
              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
              "operator": "String",
              "firstOperand": {
                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                "operator": "String",
                "firstOperand": {
                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                  "operator": "String",
                  "firstOperand": {
                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                    "operator": "String",
                    "firstOperand": {
                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                      "operator": "String",
                      "firstOperand": {
                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                        "operator": "String",
                        "firstOperand": {
                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                          "operator": null,
                          "firstOperand": null,
                          "secondOperand": {
                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                            "operator": null,
                            "firstOperand": null,
                            "secondOperand": {
                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                              "operator": null,
                              "firstOperand": null,
                              "secondOperand": {
                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                "operator": null,
                                "firstOperand": null,
                                "secondOperand": {
                                  "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                  "operator": null,
                                  "firstOperand": null,
                                  "secondOperand": {
                                    "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                    "operator": null,
                                    "firstOperand": null,
                                    "secondOperand": {
                                      "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                      "operator": null,
                                      "firstOperand": null,
                                      "secondOperand": {
                                        "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                        "operator": null,
                                        "firstOperand": null,
                                        "secondOperand": {
                                          "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                          "operator": null,
                                          "firstOperand": null,
                                          "secondOperand": {
                                            "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                            "operator": null,
                                            "firstOperand": null,
                                            "secondOperand": {
                                              "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                              "operator": null,
                                              "firstOperand": null,
                                              "secondOperand": {
                                                "@odata.type": "microsoft.graph.binaryManagementConditionExpression",
                                                "operator": null,
                                                "firstOperand": null,
                                                "secondOperand": null
                                              }
                                            }
                                          }
                                        }
                                      }
                                    }
                                  }
                                }
                              }
                            }
                          }
                        },
                        "secondOperand": null
                      },
                      "secondOperand": null
                    },
                    "secondOperand": null
                  },
                  "secondOperand": null
                },
                "secondOperand": null
              },
              "secondOperand": null
            },
            "secondOperand": null
          },
          "secondOperand": null
        },
        "secondOperand": null
      },
      "secondOperand": null
    },
    "secondOperand": null
  }
}
```




