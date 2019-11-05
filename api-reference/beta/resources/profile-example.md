---
title: 使用 Microsoft Graph 的个人资料 API 检索给定用户或你自己的相关信息
description: 'Microsoft Graph 应用程序可以使用个人资料 API 检索其他用户的个人资料。 '
author: kevinbellinger
localization_priority: Priority
ms.prod: people
doc_type: conceptualPageType
ms.openlocfilehash: 342eb433f7acc5c8e37d37e7ebcf7cb59f768aa1
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939248"
---
# <a name="use-the-profile-api-in-microsoft-graph-to-retrieve-information-about-yourself-or-another-user"></a><span data-ttu-id="d0a68-103">使用 Microsoft Graph 的个人资料 API 检索你自己或其他用户的相关信息</span><span class="sxs-lookup"><span data-stu-id="d0a68-103">Use the Profile API in Microsoft Graph to retrieve information about yourself or another user</span></span> 

<span data-ttu-id="d0a68-104">Microsoft Graph 应用程序可以使用个人资料 API 检索已登录用户或具有有效 Azure AD 或 Microsoft 帐户的其他用户的个人资料。</span><span class="sxs-lookup"><span data-stu-id="d0a68-104">Microsoft Graph applications can use the Profile API to retrieve the profile of the signed-in user or another user with a valid Azure AD or Microsoft account.</span></span> <span data-ttu-id="d0a68-105">可以在应用程序中使用此信息，以便于将其他用户置于上下文中考虑，在应用程序内为此用户提供更加丰富的体验，或用作用于存储用户的扩展信息的机制（也可在 Microsoft 365 中使用它）。</span><span class="sxs-lookup"><span data-stu-id="d0a68-105">This information can be used in applications to assist in contextualizing another user, providing a richer experience for the user within the application or as a mechanism for storing extended information about the user which can also be used within Microsoft 365.</span></span> 

## <a name="authorization"></a><span data-ttu-id="d0a68-106">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0a68-106">Authorization</span></span>

<span data-ttu-id="d0a68-107">若要在 Microsoft Graph 中调用 People API，应用必须拥有适当的权限：</span><span class="sxs-lookup"><span data-stu-id="d0a68-107">To call the People API in Microsoft Graph, your app will need the appropriate permissions:</span></span>

* <span data-ttu-id="d0a68-108">User.Read - 用于进行常规的个人资料 API 调用；例如 `https://graph.microsoft.com/beta/me/profile/`。</span><span class="sxs-lookup"><span data-stu-id="d0a68-108">People.Read - Use to make general People API calls; for example, `https://graph.microsoft.com/beta/me/profile/`. People.Read requires end user consent.</span></span> <span data-ttu-id="d0a68-109">User.Read 需要获得最终用户的同意。</span><span class="sxs-lookup"><span data-stu-id="d0a68-109">User.Read requires end user consent.</span></span>

## <a name="view-my-profile"></a><span data-ttu-id="d0a68-110">查看我的个人资料</span><span class="sxs-lookup"><span data-stu-id="d0a68-110">View my profile</span></span>

<span data-ttu-id="d0a68-111">此部分中的请求可以获取与登录用户 (`/me`) 相关度最高的人员。</span><span class="sxs-lookup"><span data-stu-id="d0a68-111">The requests in this section get the people most relevant to the signed-in user (`/me`).</span></span> <span data-ttu-id="d0a68-112">这些请求要求已登录用户具有 User.Read 权限。</span><span class="sxs-lookup"><span data-stu-id="d0a68-112">These requests require the User.Read permission to be present for the signed-in user.</span></span> 


```http
GET https://graph.microsoft.com/beta/me/profile/
```

<span data-ttu-id="d0a68-p104">以下示例显示了相应的响应。默认情况下，每个响应返回 10 个记录。可以使用 *$top* 查询参数更改此设置。本示例使用 *$top* 将响应限制为三个记录。</span><span class="sxs-lookup"><span data-stu-id="d0a68-p104">The following example shows the response. By default, each response returns 10 records. You can change this by using the *$top* query parameter. This example uses *$top* to limit the response to three records.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "profileId",
    "anniversaries": [],
    "websites": [],
    "educationalActivities": [
        {
            "endMonthYear": null,
            "startMonthYear": null,
            "completionMonthYear": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "c3a9f515-4a15-456b-9bf7-690dcd7f05d7",
            "program": {
                "abbreviation": null,
                "description": null,
                "displayName": "",
                "grade": null,
                "notes": null,
                "webUrl": null
            },
            "institution": {
                "description": null,
                "displayName": "Colorado State University",
                "location": null,
                "webUrl": null
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "emails": [
        {
            "address": "john.doe@contoso.com",
            "displayName": null,
            "type": "main",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "046452c0-c893-4fd1-a7ca-57e2ccf13861",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "interests": [
        {
            "categories": [],
            "description": null,
            "displayName": "Microsoft Graph",
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0c568cf5-5e44-4b3e-aefd-6b46ca00a880",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "languages": [
        {
            "displayName": "English (United States)",
            "tag": "en-US",
            "proficiency": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "3d34dc2e-fc84-43ff-98f6-884467caba72",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],

    "names": [
        {
            "displayName": "John Doe",
            "first": "John",
            "initials": "JD",
            "last": "Doe",
            "languageTag": null,
            "maiden": null,
            "middle": null,
            "nickname": null,
            "suffix": null,
            "title": null,
            "pronunciation": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "b79302ca-7f05-4c89-96ce-b89d5855eb0e",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "phones": [
        {
            "displayName": null,
            "type": "business",
            "number": "+47 (9) 387654321",
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d22aef2c-f332-4958-aac3-8d1d710a9e32",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "positions": [
        {
            "categories": [],
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "0f4d49c8-76cb-4d56-9f92-a10e182ba0e1",
            "detail": {
                "description": null,
                "endMonthYear": "0001-01-01",
                "jobTitle": "Associate Architect",
                "startMonthYear": "0001-01-01",
                "summary": null,
                "company": {
                    "displayName": "Contoso Corporation",
                    "pronunciation": null,
                    "department": "Architecture",
                    "officeLocation": "",
                    "webUrl": null,
                    "address": {
                        "type": "business",
                        "postOfficeBox": null,
                        "street": "",
                        "city": "Oslo",
                        "state": "",
                        "countryOrRegion": "",
                        "postalCode": ""
                    }
                }
            },
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "AAD",
                    "id": null
                }
            }
        }
    ],
    "projects": [
        {
            "categories": [],
            "client": null,
            "displayName": "Profile on Graph",
            "detail": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "d6d84567-513a-47be-9be2-99fee6a12777",
            "colleagues": [],
            "sponsors": [],
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "skills": [
        {
            "categories": [],
            "displayName": "REST API Design",
            "proficiency": null,
            "webUrl": null,
            "allowedAudiences": "everyone",
            "createdDateTime": "0001-01-01T00:00:00Z",
            "inference": null,
            "lastModifiedDateTime": "0001-01-01T00:00:00Z",
            "id": "9cd979f9-7a43-4dd1-a628-42bb07bd0974",
            "createdBy": {
                "device": null,
                "user": null,
                "application": {
                    "displayName": "UPA",
                    "id": null
                }
            }
        }
    ],
    "webAccounts": []
}
```
