---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9d05701a1a5a44af3931d3407d9c2aab413af80
ms.sourcegitcommit: 5bb981b4853663354a566d4a4a5cbf288939e441
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2021
ms.locfileid: "53581254"
---
```objc

MSHTTPClient *httpClient = [MSClientFactory createHTTPClientWithAuthenticationProvider:authenticationProvider];

NSString *MSGraphBaseURL = @"https://graph.microsoft.com/beta/";
NSMutableURLRequest *urlRequest = [NSMutableURLRequest requestWithURL:[NSURL URLWithString:[MSGraphBaseURL stringByAppendingString:@"/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/b2eba9a1-b357-42ee-83a8-336522ed6cbf"]]];
[urlRequest setHTTPMethod:@"PUT"];
[urlRequest setValue:@"application/json" forHTTPHeaderField:@"Content-Type"];

MSGraphAccessPackageAssignmentPolicy *accessPackageAssignmentPolicy = [[MSGraphAccessPackageAssignmentPolicy alloc] init];
[accessPackageAssignmentPolicy setId:@"b2eba9a1-b357-42ee-83a8-336522ed6cbf"];
[accessPackageAssignmentPolicy setAccessPackageId:@"4c02f928-7752-49aa-8fc8-e286d973a965"];
[accessPackageAssignmentPolicy setDisplayName:@"All Users"];
[accessPackageAssignmentPolicy setDescription:@"All users can request for access to the directory."];
[accessPackageAssignmentPolicy setCanExtend: false];
[accessPackageAssignmentPolicy setDurationInDays: 365];
[accessPackageAssignmentPolicy setExpirationDateTime: null];
MSGraphRequestorSettings *requestorSettings = [[MSGraphRequestorSettings alloc] init];
[requestorSettings setScopeType:@"AllExistingConnectedOrganizationSubjects"];
[requestorSettings setAcceptRequests: true];
NSMutableArray *allowedRequestorsList = [[NSMutableArray alloc] init];
[requestorSettings setAllowedRequestors:allowedRequestorsList];
[accessPackageAssignmentPolicy setRequestorSettings:requestorSettings];
MSGraphApprovalSettings *requestApprovalSettings = [[MSGraphApprovalSettings alloc] init];
[requestApprovalSettings setIsApprovalRequired: true];
[requestApprovalSettings setIsApprovalRequiredForExtension: false];
[requestApprovalSettings setIsRequestorJustificationRequired: true];
[requestApprovalSettings setApprovalMode:@"SingleStage"];
NSMutableArray *approvalStagesList = [[NSMutableArray alloc] init];
MSGraphApprovalStage *approvalStages = [[MSGraphApprovalStage alloc] init];
[approvalStages setApprovalStageTimeOutInDays: 14];
[approvalStages setIsApproverJustificationRequired: true];
[approvalStages setIsEscalationEnabled: false];
[approvalStages setEscalationTimeInMinutes: 11520];
NSMutableArray *primaryApproversList = [[NSMutableArray alloc] init];
MSGraphUserSet *primaryApprovers = [[MSGraphUserSet alloc] init];
[primaryApprovers setIsBackup: true];
[primaryApprovers setId:@"d2dcb9a1-a445-42ee-83a8-476522ed6cbf"];
[primaryApprovers setDescription:@"group for users from connected organizations which have no external sponsor"];
[primaryApproversList addObject: primaryApprovers];
MSGraphUserSet *primaryApprovers = [[MSGraphUserSet alloc] init];
[primaryApprovers setIsBackup: false];
[primaryApproversList addObject: primaryApprovers];
[approvalStages setPrimaryApprovers:primaryApproversList];
[approvalStagesList addObject: approvalStages];
[requestApprovalSettings setApprovalStages:approvalStagesList];
[accessPackageAssignmentPolicy setRequestApprovalSettings:requestApprovalSettings];
NSMutableArray *questionsList = [[NSMutableArray alloc] init];
MSGraphAccessPackageQuestion *questions = [[MSGraphAccessPackageQuestion alloc] init];
[questions setIsRequired: false];
MSGraphAccessPackageLocalizedContent *text = [[MSGraphAccessPackageLocalizedContent alloc] init];
[text setDefaultText:@"what state are you from?"];
NSMutableArray *localizedTextsList = [[NSMutableArray alloc] init];
MSGraphAccessPackageLocalizedText *localizedTexts = [[MSGraphAccessPackageLocalizedText alloc] init];
[localizedTexts setText:@"¿De qué estado eres?"];
[localizedTexts setLanguageCode:@"es"];
[localizedTextsList addObject: localizedTexts];
[text setLocalizedTexts:localizedTextsList];
[questions setText:text];
NSMutableArray *choicesList = [[NSMutableArray alloc] init];
MSGraphAccessPackageAnswerChoice *choices = [[MSGraphAccessPackageAnswerChoice alloc] init];
[choices setActualValue:@"AZ"];
MSGraphAccessPackageLocalizedContent *displayValue = [[MSGraphAccessPackageLocalizedContent alloc] init];
NSMutableArray *localizedTextsList = [[NSMutableArray alloc] init];
MSGraphAccessPackageLocalizedText *localizedTexts = [[MSGraphAccessPackageLocalizedText alloc] init];
[localizedTexts setText:@"Arizona"];
[localizedTexts setLanguageCode:@"es"];
[localizedTextsList addObject: localizedTexts];
[displayValue setLocalizedTexts:localizedTextsList];
[choices setDisplayValue:displayValue];
[choicesList addObject: choices];
MSGraphAccessPackageAnswerChoice *choices = [[MSGraphAccessPackageAnswerChoice alloc] init];
[choices setActualValue:@"CA"];
MSGraphAccessPackageLocalizedContent *displayValue = [[MSGraphAccessPackageLocalizedContent alloc] init];
NSMutableArray *localizedTextsList = [[NSMutableArray alloc] init];
MSGraphAccessPackageLocalizedText *localizedTexts = [[MSGraphAccessPackageLocalizedText alloc] init];
[localizedTexts setText:@"California"];
[localizedTexts setLanguageCode:@"es"];
[localizedTextsList addObject: localizedTexts];
[displayValue setLocalizedTexts:localizedTextsList];
[choices setDisplayValue:displayValue];
[choicesList addObject: choices];
[questions setChoices:choicesList];
[questions setAllowsMultipleSelection: false];
[questionsList addObject: questions];
MSGraphAccessPackageQuestion *questions = [[MSGraphAccessPackageQuestion alloc] init];
[questions setIsRequired: false];
MSGraphAccessPackageLocalizedContent *text = [[MSGraphAccessPackageLocalizedContent alloc] init];
[text setDefaultText:@"Who is your manager?"];
NSMutableArray *localizedTextsList = [[NSMutableArray alloc] init];
MSGraphAccessPackageLocalizedText *localizedTexts = [[MSGraphAccessPackageLocalizedText alloc] init];
[localizedTexts setText:@"por qué necesita acceso a este paquete"];
[localizedTexts setLanguageCode:@"es"];
[localizedTextsList addObject: localizedTexts];
[text setLocalizedTexts:localizedTextsList];
[questions setText:text];
[questions setIsSingleLineQuestion: false];
[questionsList addObject: questions];
[accessPackageAssignmentPolicy setQuestions:questionsList];

NSError *error;
NSData *accessPackageAssignmentPolicyData = [accessPackageAssignmentPolicy getSerializedDataWithError:&error];
[urlRequest setHTTPBody:accessPackageAssignmentPolicyData];

MSURLSessionDataTask *meDataTask = [httpClient dataTaskWithRequest:urlRequest 
    completionHandler: ^(NSData *data, NSURLResponse *response, NSError *nserror) {

        //Request Completed

}];

[meDataTask execute];

```